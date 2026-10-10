# NOT Gate Using Verilog HDL

## Author Information

- **Name:** Shaik Mohammed Khaiser Hussain
- **Branch:** Computer Science and Engineering (CSE)

## Project Description

This project implements a NOT gate using Verilog Hardware Description Language (HDL).

A NOT gate is a digital logic circuit that reverses its input. When the input is HIGH (1), the output is LOW (0), and vice versa.

## Technologies Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- Visual Studio Code
- Git and GitHub

## Truth Table

| Input A | Output Y |
|:---:|:---:|
| 0 | 1 |
| 1 | 0 |

## Verilog Implementation

```verilog
module not_gate(
    input a,
    output y
);

assign y = ~a;

endmodule
```

## Testbench

The testbench applies both possible input values and observes the output.

## How to Run

### Compile

```bash
iverilog -o not_gate_sim not_gate.v not_gate_tb.v
```

### Simulate

```bash
vvp not_gate_sim
```

### View Waveform

```bash
gtkwave not_gate.vcd
```

## Learning Outcomes

- Understanding NOT gate logic.
- Learning the Verilog inversion operator.
- Writing a testbench.
- Simulating digital circuits.
- Visualizing waveforms using GTKWave.

## Project Status

Completed — basic NOT gate implementation and simulation.

---

**Author:** Shaik Mohammed Khaiser Hussain  
**Branch:** Computer Science and Engineering (CSE)