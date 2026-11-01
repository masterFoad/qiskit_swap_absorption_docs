### What should we add?

I'd like to add a pass at optimization levels 2 and 3 that moves a two-qubit gate next to a routing SWAP on the same qubit pair, when the gate commutes with everything in between. The existing two-qubit synthesis can then combine the SWAP and the gate into one block: a SWAP followed by a CX on the same pair, for example, needs 2 CX instead of 4.

Routing can leave such a gate separated from the SWAP by gates it commutes with. Here is a small example, running only the translation and optimization stages on an already-routed fragment:

```python
from qiskit import QuantumCircuit
from qiskit.transpiler import generate_preset_pass_manager

pm = generate_preset_pass_manager(2, basis_gates=["cx", "rz", "sx", "x"])

qc = QuantumCircuit(3)
qc.swap(0, 1)
qc.cz(0, 2)
qc.cp(0.7, 0, 2)
qc.cp(0.3, 0, 1)  # commutes with the two gates before it

moved = QuantumCircuit(3)
moved.swap(0, 1)
moved.cp(0.3, 0, 1)
moved.cz(0, 2)
moved.cp(0.7, 0, 2)

for c in (qc, moved):
    out = pm.optimization.run(pm.translation.run(c))
    print(out.count_ops()["cx"])
# 7
# 5
```

Moving the CP next to the SWAP saves 2 CX here. The example starts after routing because a hand-written SWAP in the input would be removed by `ElidePermutations` in the init stage. In a full `transpile()`, the SWAPs this pass works on are the ones inserted by routing, after that stage; the Benchpress numbers below are from full transpiles.

The pass would run at the start of the translation stage, after routing, while SWAPs are still explicit. It would move a gate only across operations that commute with it, keep it on its original side of the SWAP, and never move it across another SWAP.

There is a related QAOA-focused prototype in #17205 for merging RZZ gates with SWAPs during routing, with discussion moved to #17034. This proposal would work after routing, keep the router's SWAP choices, and handle other commuting two-qubit gates as well, such as CX, CZ, CP and RXX.

We tested a Python prototype of the pass on Benchpress's Qiskit transpile tests at levels 2 and 3 (1,019 cases per level, 22 skipped). The improvements were modest overall: 1.1% fewer two-qubit gates and 1.4% lower two-qubit depth (geometric mean over runs with nonzero baselines), with no count or depth regressions observed in these runs. Some circuits benefited more: at level 2 on a heavy-hex coupling map, QASMBench `qft_n63` went from 4369 to 4001 two-qubit gates (-8.4%). Median per-run transpile time increased by 2.9% at level 2 and 1.8% at level 3 (6.8% and 3.1% summed over all runs); the pass itself is written in Python, so some of this overhead may come down with a Rust implementation.
