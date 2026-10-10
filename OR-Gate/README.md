# OR Gate Using Verilog HDL

## Author Information

- **Name:** Shaik Mohammed Khaiser Hussain
- **Branch:** Computer Science and Engineering (CSE)

## Project Description

This project implements an OR gate using Verilog HDL.

An OR gate produces a HIGH output when at least one of its inputs is HIGH.

## Technologies Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- Visual Studio Code

## Truth Table

| Input A | Input B | Output Y |
|:---:|:---:|:---:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

## Verilog Implementation

```verilog
module or_gate(
    input a,
    input b,
    output y
);

assign y = a | b;

endmodule
```

## How to Run

### Compile

```bash
iverilog -o or_gate_sim or_gate.v or_gate_tb.v
```

### Simulate

```bash
vvp or_gate_sim
```

### View Waveform

```bash
gtkwave or_gate.vcd
```

## Learning Outcomes

- Understanding OR logic.
- Writing Verilog modules.
- Creating testbenches.
- Simulating digital circuits.
- Visualizing waveforms.