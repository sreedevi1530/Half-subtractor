# Half Subtractor using Verilog

## Overview
A Half Subtractor is a combinational logic circuit that subtracts one binary digit from another. It has two inputs (A and B) and two outputs:

- Difference (D)
- Borrow (Bo)

This project implements a Half Subtractor using Verilog HDL and verifies its functionality using a testbench.

---

## Truth Table

| A | B | Difference | Borrow |
|---|---|------------|---------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |

---

## Boolean Expressions

Difference = A XOR B

Borrow = (~A) AND B

---

## Files

- `half_subtractor.v` – Verilog design module
- `half_subtractor_tb.v` – Testbench
- `output.png` – Simulation waveform
- `README.md` – Project documentation

---

## Simulation

Compile and simulate using ModelSim, Vivado, Icarus Verilog, or EDA Playground.

Example (Icarus Verilog):

```bash
iverilog -o half_subtractor half_subtractor.v half_subtractor_tb.v
vvp half_subtractor
```

---

## Expected Output

```
A=0 B=0 Difference=0 Borrow=0
A=0 B=1 Difference=1 Borrow=1
A=1 B=0 Difference=1 Borrow=0
A=1 B=1 Difference=0 Borrow=0
```

---

## Author

Deepthi