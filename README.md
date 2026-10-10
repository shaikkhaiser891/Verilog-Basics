# 🚀 Verilog Basics — Digital Logic Design

Welcome to my **Verilog Basics** repository! This project documents my journey of learning Verilog HDL and designing digital logic circuits, from fundamental logic gates to more advanced digital systems.

## 👨‍🎓 Author Information

- **Name:** Shaik Mohammed Khaiser Hussain
- **Branch:** Computer Science and Engineering (CSE)
- **Project:** Verilog Basics — Digital Logic Design

## 📌 About the Project

The goal of this repository is to practice Verilog programming, understand digital hardware design, and simulate circuits to verify their functionality.

This repository will be continuously updated as I learn new concepts and develop additional projects.

## 🛠️ Technologies & Tools

- **Verilog HDL** — Hardware Description Language
- **Icarus Verilog** — Compilation and simulation
- **GTKWave** — Waveform visualization
- **Git** — Version control
- **GitHub** — Project hosting and collaboration
- **Visual Studio Code** — Code editor

## 📂 Project Structure

```text
Verilog-Basics/
│
├── README.md
├── and_gate.v
└── and_gate_tb.v
```

### File Descriptions

| File | Description |
|---|---|
| `README.md` | Project overview and documentation |
| `and_gate.v` | Verilog implementation of an AND gate |
| `and_gate_tb.v` | Testbench for verifying the AND gate |

## 🔌 Project 1: AND Gate

An AND gate is a fundamental digital logic circuit. Its output is HIGH (`1`) only when both inputs are HIGH (`1`).

### Verilog Implementation

```verilog
module and_gate(
    input a,
    input b,
    output y
);

assign y = a & b;

endmodule
```

### Truth Table

| Input A | Input B | Output Y |
|:---:|:---:|:---:|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

## 🧪 Simulation

The AND gate can be tested using a Verilog testbench and simulated with Icarus Verilog.

### Compile the Design

```bash
iverilog -o and_gate_sim and_gate.v and_gate_tb.v
```

### Run the Simulation

```bash
vvp and_gate_sim
```

### View the Waveform

The testbench generates a Value Change Dump (VCD) file named `and_gate.vcd`.

Open the waveform using:

```bash
gtkwave and_gate.vcd
```

GTKWave allows you to visualize the inputs and output over simulation time.

## 🎯 Learning Objectives

- Understand Verilog syntax and module structure.
- Learn digital logic gates and Boolean expressions.
- Develop and simulate digital circuits.
- Write testbenches to verify hardware behavior.
- Analyze waveforms using GTKWave.
- Practice Git and GitHub for version control.

## 🗺️ Future Plans

As I continue learning, I plan to add the following designs:

- [ ] AND, OR, NOT, NAND, NOR, and XOR gates
- [ ] Half Adder
- [ ] Full Adder
- [ ] Multiplexer and Demultiplexer
- [ ] Encoder and Decoder
- [ ] Flip-Flops
- [ ] Counters and Registers
- [ ] Finite State Machines (FSMs)
- [ ] Traffic Light Controller
- [ ] Digital Clock

## 📈 Progress

This repository is a work in progress. New designs, testbenches, and simulation examples will be added as I develop my Verilog skills.

## 🤝 Contributions

Suggestions, feedback, and ideas for improving these learning projects are welcome.

## 📜 License

This project is intended for educational and learning purposes.