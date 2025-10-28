# qiskit-pi-seconds
πs units for Qiskit: 1 πs = π radians. No 2π. Clean quantum pulses.

# qiskit-pi-seconds  
**πs Units for Qiskit: Quantum Code in Native Phase-Time**  

> `1 πs ≜ π / ω` → **π radians of phase**  
> X-gate = `rx_pi(1, 0)` | Full cycle = `delay_pi(2, 0)` | **No 2π clutter**

**By [YOUR NAME] – Outsider Hacker** | October 2025  

---

## Why This Exists  
In quantum control, **phase is everything** — but we hide π behind 2π.  
This extension makes **π the unit**, not a fraction.

```python
from qiskit import QuantumCircuit
from pi_seconds import πs

qc = QuantumCircuit(1)
qc.rx_pi(1, 0)      # X-gate: 1 πs
qc.delay_pi(2, 0)   # Wait 1 full cycle
qc.rx_pi(1, 0)      # Back to |0>
