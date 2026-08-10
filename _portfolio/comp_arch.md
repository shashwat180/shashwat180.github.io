---
title: "Architectural Modeling of Superscalar OoO Execution & Matrix Accelerators"
excerpt: "Developed cycle-accurate C++ simulators to model superscalar out-of-order CPU execution and systolic-array GEMM accelerators, evaluating architectural performance through instruction-level profiling and hardware parameter scaling.<br/><img src='/images/comp_arch.png'>"
collection: portfolio
---

<h2>Overview</h2>
To deeply understand the bottlenecks and design trade-offs in modern processing systems, I developed custom, cycle-accurate simulators in C++. This project encompassed two distinct architectural models: a high-performance superscalar out-of-order (OoO) CPU and a specialized systolic-array accelerator for General Matrix Multiply (GEMM) operations.

<h2>Superscalar Out-of-Order CPU Modeling</h2>
I engineered a comprehensive CPU simulator that accurately mimics the complex data and control flow of a modern processor.

<ul>
    <li>Pipeline Implementation: The design features a fully functional instruction pipeline, including advanced hazard resolution, pipeline data forwarding, and branch prediction mechanisms.</li>

<li>Instruction Scheduling: To model out-of-order execution, I implemented dynamic scheduling components, specifically a Register Alias Table (RAT) for register renaming and a Reorder Buffer (ROB) to ensure precise state management and in-order retirement.</li></ul>

<h2>Systolic-Array GEMM Accelerator</h2>
In parallel with the CPU model, I built a systolic-array simulator specifically tailored to execute matrix multiplication workloads. This model allowed me to isolate and study key hardware constraints, such as the impact of FIFO buffer sizing and off-chip memory bandwidth scaling on overall cycles-to-completion.

<h2>Architectural Performance Evaluation</h2>
To validate and analyze both designs, I processed real-world instruction traces through the simulators. I systematically evaluated the architectural performance of the models by extracting and analyzing core metrics, including Cycles Per Instruction (CPI), overall pipeline utilization, and branch misprediction rates, using the data to identify structural bottlenecks within the designs.
