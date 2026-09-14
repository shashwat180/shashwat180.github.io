---
title: "RV32I CPU Design using Python and SystemVerilog"
excerpt: "Developed a Python-based Instruction Set Simulator for the full RV32I base integer architecture as a golden reference model, and am translating it into synthesizable SystemVerilog RTL with an automated Cocotb verification environment.<br/><img src='/images/rv32i_cpu.jpg'>"
collection: portfolio
---

<h2>Overview</h2>
To gain a ground-up understanding of processor design, I am building a RISC-V CPU implementing the complete RV32I base integer instruction set, spanning the full pipeline from a software reference model to synthesizable hardware. The project is structured in two phases: first establishing a golden functional reference in Python, then translating that architecture into RTL for hardware validation.

<h2>Instruction Set Simulator (Golden Reference)</h2>
I developed a Python-based Instruction Set Simulator (ISS) implementing all 38 instructions of the RV32I base integer architecture. This involved modeling the core microarchitectural components—registers, memory, and the instruction execution pipeline—entirely in software, establishing a golden reference standard against which the hardware implementation could later be validated for correctness.

<h2>RTL Development</h2>
Building on the validated architectural model, I am translating the high-level ISS into synthesizable SystemVerilog RTL, implementing the CPU datapath and control logic in hardware. This phase focuses on faithfully mapping the golden reference's behavior into a physically realizable design suitable for synthesis and deployment.

<h2>Functional Verification</h2>
To ensure strict compliance with the RISC-V ISA, I am developing an automated verification environment using Cocotb and Icarus Verilog. This environment runs the SystemVerilog RTL against the Python golden reference model, enabling automated functional testing across the full instruction set and catching correctness issues early in the hardware development cycle.
