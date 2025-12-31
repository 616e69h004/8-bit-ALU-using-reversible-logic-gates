# Design and Implementation of a VLSI-Based Low-Power 8-Bit ALU Using Reversible Logic Gates

## Overview
This repository presents an academic major project focused on the **design and implementation of a VLSI-based low-power 8-bit Arithmetic Logic Unit (ALU) using reversible logic gates**.  
The project is aimed at demonstrating strong fundamentals in **VLSI design, low-power CMOS circuits, and reversible/quantum-inspired computation**, and is intended for evaluation by **professors, researchers, and industry recruiters**.

Reversible logic preserves information by ensuring a one-to-one mapping between inputs and outputs. According to **Landauer’s principle**, information loss leads to unavoidable energy dissipation, while **Bennett’s principle** shows that reversible computation can theoretically eliminate this loss. This project applies these principles to practical CMOS VLSI design using **Cadence Virtuoso**.

---

## Key Contributions
- Complete **8-bit reversible ALU architecture**
- Transistor-level design using **180 nm CMOS technology**
- Extensive use of **reversible logic gates** for low-power operation
- Fully simulated and verified using **Cadence Virtuoso (ADE + ViVA)**

---

## Reversible Gates Implemented
All gates were designed at the **transistor level** using **CMOS transmission-gate (pass transistor) logic**:

- **Feynman Gate (CNOT)** – Signal copying and XOR
- **Toffoli Gate (CCNOT)** – Universal reversible gate
- **Fredkin Gate** – Controlled swap / conservative logic
- **Peres Gate** – Combined XOR and AND with low quantum cost
- **DKG Gate** – Optimized 4×4 gate for adders and subtractors
- **TR Gate (Thapliyal–Ranganathan)** – Arithmetic and comparator logic
- **BJN Gate (Bruce–Jha–Nayeem)** – Optimized comparator and arithmetic gate

Each gate was individually verified using transient simulations.

---

## ALU Functional Blocks
The reversible ALU consists of the following modules:

- **8-bit Reversible Adder**
  - Built using cascaded **DKG-based full adders**
- **8-bit Reversible Subtractor**
  - Uses the same DKG structure with modified control inputs
- **2-bit Reversible Multiplier**
  - Implemented using **Peres gates** for partial product generation
- **8-bit Reversible Comparator**
  - Designed using **TR and BJN gates**
- **Reversible Control Logic**
  - Selects arithmetic and logic operations without information loss

---

## Technology and Design Details
- **Technology Node:** 180 nm CMOS
- **Supply Voltage:** 1.8 V
- **Logic Style:** CMOS Transmission Gate / Pass Transistor Logic
- **Design Level:** Transistor-level schematics
- **Verification:** Transient and DC simulations
- **Tools Used:** Cadence Virtuoso, ADE, ViVA

Design emphasis was placed on:
- Full voltage swing
- Low power dissipation
- Minimal garbage outputs
- Logical reversibility
- Stable waveform behavior

---

## How to Run Simulations (Cadence Virtuoso)
1. Open **Cadence Virtuoso**
2. Load the **180 nm CMOS PDK**
3. Open the required schematic (gate or ALU block)
4. Apply input vectors using voltage sources or pattern generators
5. Run **Transient Analysis** in ADE
6. Verify outputs in **ViVA waveform viewer**
7. Compare outputs with reversible truth tables

---

## Learning Outcomes
This project demonstrates proficiency in:
- VLSI transistor-level design
- Low-power CMOS logic
- Reversible and quantum-inspired computing
- Cadence Virtuoso workflow
- Digital arithmetic circuit design
- Power-aware hardware architecture

---

## Future Scope
- Complete and optimize the **8-bit reversible comparator**
- Perform **layout, DRC, and LVS**
- Fabrication and silicon-level validation
- Extension to **quantum circuit models**
- Comparative benchmarking with irreversible ALUs
- Scaling to 16-bit / 32-bit reversible processors

---

## Academic Context
- **Degree:** B.Tech in Electrical and Electronics Engineering
- **Project Type:** Major Project
- **Domain:** VLSI, Low-Power Design, Reversible Logic, Quantum Computing Foundations

---

> This repository is intended to showcase **design depth, theoretical understanding, and practical VLSI skills**, rather than being a plug-and-play software project.
