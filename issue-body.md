### What should we add?

I'd like to add a commutation-based reordering pass at optimization levels 2 and 3 that moves a two-qubit gate next to a routing SWAP on the same physical qubit pair. The existing two-qubit synthesis can then optimize the SWAP and the gate as one block instead of two.

Routing can leave a gate separated from a SWAP by gates that commute with it. For example, consider this fragment of an already-routed circuit, running only the translation and optimization stages:

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

The last CP commutes with the intervening CZ and CP, so it can move directly after the SWAP, and the optimization stage can then synthesize the SWAP and CP as one block, saving 2 CX here. The saving is easiest to see with a CX: a SWAP followed immediately by a CX on the same ordered pair synthesizes to two CX gates instead of four.

The pass would run at the start of the translation stage, after routing, while SWAPs are still explicit. It would move a gate only across operations that commute with it, keep it on its original side of the SWAP, and never move it across another SWAP.

On Benchpress's Qiskit transpile tests at levels 2 and 3 (1,019 cases per level), a Python prototype of the pass gave:

- 1.1% fewer two-qubit gates and 1.4% lower two-qubit depth (geometric mean over runs with nonzero baselines).
- Fewer two-qubit gates in about a third of the runs, with no count or depth regressions observed.
- Larger gains on some circuits, such as QFT: at level 2 on a heavy-hex coupling map, QASMBench `qft_n63` went from 4369 to 4001 two-qubit gates (-8.4%).
- Median per-run transpile time +2.9% at level 2 and +1.8% at level 3 (+6.8% and +3.1% in total).

Related to #17205 (discussion moved to #17034), which proposes merging RZZ gates with SWAPs during QAOA routing. This pass would run after routing and leave the router's SWAP choices unchanged. It would also handle gates such as CX, CZ, CP and RXX when they commute with the operations in between.

### AI disclosure

I developed this as part of IBM Research's Spotlights project on AI-native software optimization. I used Claude Code and OpenAI Codex to develop, test and review the implementation.