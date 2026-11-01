### What should we add?

I'd like to add a commutation-based reordering pass at optimization levels 2 and 3 that moves a two-qubit gate next to a routing SWAP on the same physical qubit pair. The existing two-qubit synthesis can then optimize the SWAP and the gate as one block instead of two.

Routing can leave an gate separated from a SWAP by gates that commute with it. For example, consider this fragment of an already-routed circuit:

```python
from qiskit import QuantumCircuit

qc = QuantumCircuit(3)
qc.swap(0, 1)
qc.rz(0.2, 0)
qc.cz(0, 2)
qc.cp(0.3, 0, 1)
qc.cx(0, 2)
qc.cx(1, 2)
```

The CP commutes with the intervening RZ and CZ, so it can move directly after the SWAP, and the optimization stage can then synthesize the SWAP and CP as one block. The saving is easiest to see with a CX: a SWAP followed immediately by a CX on the same ordered pair synthesizes to two CX gates instead of four.

The pass would run at the start of the translation stage, after routing, while SWAPs are still explicit. It would move an gate only across operations that commute with it on every shared wire, keep it on its original side of the SWAP, and never move it across another SWAP. 

On a collection of Qiskit's benchmarks, this gave 3.93% lower two-qubit depth and 2.85% fewer two-qubit gates, at 1.61% higher transpilation runtime. 

### AI disclosure

I developed this as part of IBM Research's Spotlights project on AI-native software optimization. I used Claude Code and OpenAI Codex to develop, test and review the implementation.
