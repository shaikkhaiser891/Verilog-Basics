# OR Gate Using Verilog HDL

## Author Information

- **Name:** Shaik Mohammed Khaiser Hussain
- **Branch:** Computer Science and Engineering (CSE)

## Project Description

This project implements a basic OR gate using Verilog Hardware Description Language (HDL).

An OR gate produces a HIGH output (`1`) when at least one of its inputs is HIGH (`1`). The output is LOW (`0`) only when both inputs are LOW (`0`).

## Technologies Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- Visual Studio Code
- Git and GitHub

## Truth Table

| Input A | Input B | Output Y |
|:---:|:---:|:---:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

## Verilog Implementation

Create a file named `or_gate.v`.

```verilog
module or_gate(
    input a,
    input b,
    output y
);

assign y = a | b;

endmodule
```

## Testbench

Create a file named `or_gate_tb.v`.

```verilog
`timescale 1ns/1ps

module or_gate_tb;

reg a, b;
wire y;

or_gate uut (
    .a(a),
    .b(b),
    .y(y)
);

initial begin
    $dumpfile("or_gate.vcd");
    $dumpvars(0, or_gate_tb);

    $monitor("Time=%0t | A=%b B=%b Y=%b",
             $time, a, b, y);

    a = 0; b = 0;
    #10;

    a = 0; b = 1;
    #10;

    a = 1; b = 0;
    #10;

    a = 1; b = 1;
    #10;

    $finish;
end

endmodule
```

## How to Run

Open Command Prompt inside the `OR-Gate` project folder.

### 1. Compile the Verilog Code

```bash
iverilog -o or_gate_sim or_gate.v or_gate_tb.v
```

### 2. Run the Simulation

```bash
vvp or_gate_sim
```

### 3. View the Waveform

```bash
gtkwave or_gate.vcd
```

The waveform allows you to observe how the inputs and output change over simulation time.

## Expected Output

| Input A | Input B | Output Y |
|:---:|:---:|:---:|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

## Learning Outcomes

- Understanding OR logic and Boolean expressions.
- Writing Verilog modules.
- Creating testbenches.
- Compiling and simulating digital circuits.
- Visualizing signal waveforms using GTKWave.
- Managing source code using Git and GitHub.

## Future Improvements

- Implement additional logic gates.
- Design half adders and full adders.
- Develop multiplexers and demultiplexers.
- Explore sequential circuits and counters.

## Project Status

Completed — basic OR gate implementation and simulation.

---

**Author:** Shaik Mohammed Khaiser Hussain  
**Branch:** Computer Science and Engineering (CSE)