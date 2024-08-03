# MIPS 32-Bit CPU Using Logisim

This repository contains the design and simulation of a subset of the MIPS 32-bit architecture using Logisim. The project aims to implement a 32-bit pipelined version of the MIPS architecture to execute basic MIPS instructions.

## Description

The MIPS (Microprocessor without Interlocked Pipeline Stages) architecture is a RISC (Reduced Instruction Set Computing) architecture that is widely used in academic settings to teach CPU design. This project focuses on designing the datapath and control units of a MIPS CPU, implementing a pipelined architecture to enhance instruction execution efficiency.

## Tools and Requirements

- **Logisim:** A graphical tool for designing and simulating digital logic circuits.
  - Download and install Logisim from the [official website](http://www.cburch.com/logisim/).

## Features

- **32-Bit Pipelined MIPS CPU:** A complete design and simulation of a pipelined MIPS CPU.
- **Instruction Set:** Supports a subset of MIPS instructions for basic operations.
- **Modular Design:** The CPU is designed using modular components for better understanding and scalability.
- **Datapath and Control Units:** Detailed design of the datapath and control units to handle instruction execution.

## Getting Started

### Prerequisites

Ensure you have Logisim installed on your system.

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/jubayer98/Design-Simulate-A-MIPS-32-Bit-CPU-Using-Logisim.git
   cd Design-Simulate-A-MIPS-32-Bit-CPU-Using-Logisim
   ```

2. **Open in Logisim:**
   - Launch Logisim.
   - Open the project file (`cpu.circ`) in Logisim.

## Usage

1. **Simulation:**
   - Once the project is open in Logisim, start the simulation by clicking on the "Simulate" menu and selecting "Ticks Enabled".
   - Load the machine code into the instruction memory and observe the execution of instructions through the pipeline stages.

2. **Customization:**
   - The modular design allows you to modify and extend the CPU easily.
   - You can add more instructions or optimize the pipeline stages for better performance.

## How It Works

### Example

Let's consider an example of adding two numbers:

- **C Code:**
  ```c
  A = B + C;
  ```

- **Assembly Code:**
  ```assembly
  add a, b, c  # a is the sum of b and c
  ```

- **Machine Code:**
  ```binary
  000000 10001 10010 01000 00000 100000
  ```

### Datapath

The datapath of the MIPS CPU includes the following components:

- **Program Counter (PC):** Holds the address of the next instruction to be executed.
- **Instruction Memory:** Stores the instructions to be executed.
- **Register File:** Contains the general-purpose registers for storing operands and results.
- **ALU (Arithmetic Logic Unit):** Performs arithmetic and logical operations.
- **Data Memory:** Stores data that is read from or written to by the instructions.
- **Pipeline Registers:** Store intermediate values between pipeline stages.

### Control Unit

The control unit generates the necessary control signals to coordinate the operations of the datapath components. It ensures that instructions are executed correctly through the pipeline stages.

## Contributing

Contributions are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request.

---

Thank you for using the MIPS 32-Bit CPU simulation project. We hope it enhances your understanding of CPU design and the MIPS architecture.
