# Half Adder using Verilog

## Overview
This project implements a Half Adder using Verilog HDL. A Half Adder performs the addition of two single-bit binary numbers and produces a Sum and a Carry output.

## Truth Table

| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

## Boolean Equations

Sum = A ^ B

Carry = A & B

## Files

- `half_adder.v` : Verilog design module
- `half_adder_tb.v` : Testbench
- `simulation.png` : Simulation waveform

## Tools Used

- Verilog HDL
- ModelSim / Vivado / Icarus Verilog
- GTKWave (optional)

## Simulation

Compile:

```bash
iverilog -o half_adder half_adder.v half_adder_tb.v
```

Run:

```bash
vvp half_adder
```

View waveform:

```bash
gtkwave half_adder.vcd
```

## Expected Output

```
A B | Sum Carry
0 0 | 0    0
0 1 | 1    0
1 0 | 1    0
1 1 | 0    1
```

## Author

Your Name