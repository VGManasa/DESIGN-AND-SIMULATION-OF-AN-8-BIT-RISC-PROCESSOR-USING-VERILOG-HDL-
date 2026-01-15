# DESIGN-AND-SIMULATION-OF-AN-8-BIT-RISC-PROCESSOR-USING-VERILOG-HDL-


This project focuses on the **design, simulation, and hardware implementation** of a simple 8-bit **RISC (Reduced Instruction Set Computer) processor** using **Verilog HDL**. The processor demonstrates fundamental CPU concepts such as **instruction execution, datapath design, control logic, and hardware verification**.  

The project is **educational and portfolio-oriented**, emphasizing **clarity, modularity, and correctness** rather than high performance. It also provides hands-on experience with FPGA implementation and debugging.  

---

## Objectives

- Design a **modular 8-bit RISC architecture**.  
- Implement processor components using **Verilog HDL**.  
- Simulate and verify the processor design using **ModelSim / QuestaSim**.  
- Deploy and test the processor on the **Altera DE10 FPGA board**.  
- Visualize processor operations through **on-board LEDs, switches, and optional displays**.  
- Gain practical understanding of **CPU datapath, control signals, and instruction execution**.  

---

## Features

- **Supports basic arithmetic and logical instructions** (ADD, SUB, AND, OR, NOT, etc.)  
- Implements **load/store and branch instructions** for simple programs  
- **Modular Verilog design** for easy extension or modification  
- Real-time observation of **program execution via LEDs and switches**  
- Simulation waveforms provide **insight into instruction cycles and signal behavior**  

---

## Hardware & Tools

### Hardware

- FPGA Board: **Altera DE10**  
- FPGA Device: **Intel Cyclone**  
- Clock Source: On-board oscillator  
- I/O: LEDs, switches, optional seven-segment displays  

### Software

- **Intel Quartus Prime** for synthesis, compilation, and FPGA programming  
- **ModelSim / QuestaSim** for behavioral and timing simulations  
- **Verilog HDL** for processor design and verification  

---

## Major Components

- **Program Counter (PC)** – Keeps track of instruction addresses  
- **Instruction Memory (ROM)** – Stores the processor program  
- **Register File** – Holds general-purpose registers for operations  
- **Arithmetic Logic Unit (ALU)** – Performs arithmetic and logical computations  
- **Control Unit** – Generates control signals for instruction execution  
- **Data Memory (RAM)** – Stores data values during program execution  
- **Multiplexers and Logic Blocks** – Direct signals within the datapath  
- **Clock & Reset Circuitry** – Ensures synchronous operation and initialization  

---

## Instruction Set Architecture (ISA)

The processor implements a **reduced instruction set**, including:  

- **Data Movement:** `MOV`, `LOAD`, `STORE`  
- **Arithmetic Operations:** `ADD`, `SUB`, `INC`, `DEC`  
- **Logical Operations:** `AND`, `OR`, `XOR`, `NOT`  
- **Control Flow:** `JMP`, `JZ`, `JNZ`, `HALT`  

*(You can extend this ISA for additional functionality in future versions.)*  

---

## Simulation & Verification

- Testbenches are created in **ModelSim / QuestaSim** to verify **instruction execution**, **ALU operation**, and **register/memory updates**.  
- Waveforms provide **timing insights**, helping identify potential hazards and logic errors.  
- Simulations ensure the processor behaves as intended before FPGA deployment.  

---

## FPGA Implementation

- The design is **synthesized and mapped** to the Altera DE10 board using **Quartus Prime**.  
- **LEDs** display output or status flags, and **switches** can provide manual input.  
- Optional **seven-segment displays** show register values or program counters for debugging.  

---


## Future Enhancements

- Expand instruction set to support **multiplication, division, and more advanced branching**  
- Implement **interrupt handling** for asynchronous events  
- Integrate **peripherals** like UART, ADC/DAC, or timers  
- Optimize for **pipelining and higher performance**  

