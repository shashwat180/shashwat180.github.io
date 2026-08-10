---
title: "Efficient Delay Fault Simulation for Short Defects in Standard Cells"
excerpt: "Conducted transistor-level reliability analysis of CMOS standard cells using Cadence and HSPICE, developing custom Python automation to model resistive shorts and characterize defect-induced timing failures. <br/><img src='/images/shorts_std_cell.PNG'>"
collection: portfolio
---

<h2>Overview</h2>
In this research project, I conducted a rigorous transistor-level reliability analysis to understand the impact of resistive shorts within CMOS standard cells. The primary objective was to accurately model defect-induced timing failures and characterize how standard cell delay fluctuates under varying defect resistances. This data is critical for establishing and supporting strict timing margin requirements in robust digital designs.

<h2>Simulation & Fault Analysis</h2>
To capture the nuanced electrical characteristics of the cells under fault conditions, I designed comprehensive testbenches using Cadence tools. I then executed extensive HSPICE simulations targeted at specific transistor-level fault locations. This allowed me to deeply analyze the behavior of the defects and observe exactly how resistive shorts propagate delay through the logic gates.

<h2>Workflow Automation</h2>
Because characterizing delays across a wide spectrum of varying defect resistances requires massive amounts of repetitive testing, I built a custom automation pipeline to scale the process. I developed Python scripts that dynamically modified the resistance values directly within the netlists, programmatically executed the batch HSPICE simulations, and automatically parsed and extracted the resulting delay metrics for final analysis.
