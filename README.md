# Quantum-Aware GAAFET Optimization Using Silvaco TCAD

<p align="center">

![Silvaco](https://img.shields.io/badge/Silvaco-ATLAS-blue)
![TCAD](https://img.shields.io/badge/TCAD-Device%20Simulation-green)
![Device](https://img.shields.io/badge/Technology-GAAFET-red)
![Focus](https://img.shields.io/badge/Focus-Low--Power%20Nanoelectronics-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

</p>

---

## Overview

This repository presents a **TCAD-based optimization of a cylindrical Gate-All-Around Field Effect Transistor (GAAFET)** using **Silvaco ATLAS**. Starting from a literature-based baseline device, key structural and doping parameters were optimized to improve electrostatic control and switching behavior. The optimized device was then used to implement a **low-power two-input AND gate**, demonstrating its suitability for future nanoscale digital logic applications.

The project combines **device physics, parameter optimization, quantum-aware simulation, and logic implementation**, providing a complete semiconductor device engineering workflow.

---

# Research Motivation

As CMOS technology approaches sub-5 nm technology nodes, conventional transistor architectures face severe short-channel effects and increased leakage current.

Gate-All-Around FETs (GAAFETs) provide superior electrostatic gate control by surrounding the channel on all sides, making them one of the most promising transistor architectures for next-generation low-power integrated circuits.

This project investigates how geometry scaling and doping optimization can improve GAAFET performance using TCAD simulation.

---

# Project Objectives

- Design a cylindrical nanowire GAAFET using Silvaco ATLAS
- Optimize device geometry and doping parameters
- Evaluate electrical characteristics under different bias conditions
- Compare baseline and optimized device performance
- Implement a GAAFET-based two-input AND gate
- Analyze switching characteristics and leakage behavior

---

# Device Optimization

The optimized GAAFET was obtained by modifying critical device parameters from the baseline structure.

| Parameter | Baseline | Optimized |
|-----------|----------|-----------|
| Channel Length | 200 nm | 300 nm |
| Nanowire Radius | 25 nm | 25 nm |
| Oxide Thickness | 45 nm | 6 nm |
| Source Doping | 1×10¹⁹ cm⁻³ | 5×10¹⁸ cm⁻³ |
| Drain Doping | 1×10¹⁹ cm⁻³ | 5×10¹⁹ cm⁻³ |
| Channel Doping | 1×10¹⁷ cm⁻³ | 5×10¹⁶ cm⁻³ |

---

# Optimization Strategy

The proposed optimization focuses on three key aspects:

- **Geometry Engineering**
  - Increased channel length to improve electrostatic control.
  - Reduced gate oxide thickness to strengthen gate-channel coupling.

- **Doping Engineering**
  - Optimized source, drain, and channel doping profiles.
  - Reduced channel impurity concentration to improve carrier transport.

- **Quantum-Aware Device Simulation**
  - Evaluated using advanced physical models to capture nanoscale device behavior.

---

# Simulation Workflow

```text
Baseline Device
        │
        ▼
Geometry Optimization
        │
        ▼
Doping Optimization
        │
        ▼
Mesh Generation
        │
        ▼
Quantum Physics Models
        │
        ▼
Electrical Characterization
        │
        ▼
Performance Analysis
        │
        ▼
GAAFET-Based AND Gate
```

---

# Simulation Environment

| Tool | Purpose |
|------|---------|
| Silvaco ATLAS | Device simulation |
| DeckBuild | Simulation scripting |
| TonyPlot | Visualization and analysis |
| Git | Version control |
| GitHub | Project documentation |

---

# Physical Models

The following semiconductor physics models were incorporated during simulation:

- Fermi–Dirac Statistics
- Quantum Tunneling
- Non-local Band-to-Band Tunneling (BTBT)
- Shockley–Read–Hall Recombination
- Auger Recombination
- Concentration-Dependent Mobility
- Field-Dependent Mobility
- Bandgap Narrowing

---

# Electrical Characterization

The optimized GAAFET was evaluated using standard semiconductor device metrics.

| Performance Metric |
|--------------------|
| ON-State Current (ION) |
| OFF-State Current (IOFF) |
| ON/OFF Current Ratio |
| Threshold Voltage (VTH) |
| Subthreshold Swing (SS) |
| Leakage Current |

---

# Logic Gate Verification

The optimized GAAFET was successfully employed to implement a **two-input AND gate**.

| Input A | Input B | Output |
|---------|---------|--------|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

Simulation outputs for all logic states are available in the `results/` directory.

---

# Results

The optimized device demonstrates:

- Improved electrostatic gate control
- Reduced leakage current
- Enhanced switching characteristics
- Improved gate-to-channel coupling
- Suitability for low-power nanoscale logic applications

Representative simulation results include:

- Transfer characteristics (ID–VG)
- Baseline vs optimized device comparison
- Leakage current analysis
- Logic gate verification

---

# Engineering Competencies Demonstrated

- Semiconductor Device Physics
- TCAD Device Simulation
- Silvaco ATLAS
- GAAFET Design
- Device Optimization
- Quantum Transport Modeling
- Doping Engineering
- Low-Power Logic Design
- Electrical Characterization
- Technical Documentation
- Engineering Analysis

---

# Future Work

Potential extensions of this work include:

- GAAFET-based SRAM cell design
- Ring oscillator implementation
- Sequential logic circuits
- AI-assisted device optimization
- Process variation analysis
- Sub-3 nm technology node exploration

---

# References

The publications and technical references used during this work are listed in `references.md`.


> **Disclaimer:** This repository is intended for educational and research purposes. The optimized GAAFET presented here is based on TCAD simulations and is not intended to represent a fabricated commercial device.
