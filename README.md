# Bryan Lukehart-Yun

**M.S. Mechanical Engineering — Rochester Institute of Technology (2025)**  
**Focus: Guidance, Navigation, and Control | Nonlinear Dynamics | State Estimation | Soft Robotics**

---

## About

I'm a engineer with a background spanning nonlinear system identification, derivative-free state estimation, and robotics. My work sits at the intersection of classical control theory and modern nonlinear methods from 6-DOF fixed-wing simulations to NMPC-driven soft actuator control.

My thesis focused on stable open-loop modeling and closed-loop control of McKibben Pneumatic Artificial Muscles (PAMs); a class of soft actuators where standard industry estimators (EKF, CKF) fail due to non-differentiable hysteresis dynamics. The solution required building the full GNC stack from scratch: nonlinear plant identification, derivative-free state estimation, Monte Carlo robustness validation, and real-time NMPC tracking. Validated across 11M+ samples, 16 operating conditions, and 5,520+ actuation cycles. The achieving metrics are 91% open-loop drift reduction and 1.36 mm tracking RMSE (75.6% improvement over PID).

I also speak classical aerospace GNC such as 6-DOF nonlinear truth models, linearization audits, modal stability analysis, and the full V&V workflow that flight control development requires.

Prior to graduate research, I've worked across the federal research and industry pipeline: Naval Research Laboratory (robotics integration and multiaxial test systems), Army Research Laboratory (MEMS fabrication and sensor V&V), Harvard under **Whitesides Research Group** (soft actuator fabrication), and DOW Inc. (materials testing and Python-based measurement automation).

---

## Technical Stack

| Domain | Tools |
|---|---|
| Primary Language | MATLAB, Python |
| Legacy / Simulation | Simulink |
| Embedded & Robotics | C++ |
| Control Methods | NMPC, PID, State-Space |
| Estimation | UKF, EKF, CKF |
| System ID | NLARX (Sigmoid, Wavelet, idTreePartition), Mathematical Modeling |
| Fabrication | FDM, SLA, Soft Robotics, CAD |
| Standards | ASTM C642, E2178, E2357, D143 |

---

## Featured Repositories

### [Nonlinear-Actuators-GNC-Robotics-Framework](https://github.com/BryanLukehartYun/Nonlinear-Actuators-GNC-Robotics-Framework)
Full nonlinear GNC framework for Pneumatic Artificial Muscles. Features NLARX system identification, UKF state estimation validated via Monte Carlo simulation, and NMPC achieving a 75.6% reduction in tracking error vs. baseline PID. Derived from M.S. thesis research at RIT BioSEL Lab.

### [Applied-Dynamics-and-Controls](https://github.com/BryanLukehartYun/Applied-dynamics-and-controls)
Aerospace GNC portfolio. Considered Complete: a two-part fixed-wing flight dynamics study on two module that complements each other: 6-DOF nonlinear truth model and linearization audit with full modal stability analysis and V&V overlay validation. Interplanetary mission design, orbital mechanics, and SysID modules planned.

---


## Highlights

**[Beyond Stability: NMPC Robustness Under 120% Gain Jitter](https://www.linkedin.com/posts/bryan-lukehart-yun_gnc-robotics-controltheory-activity-7435046592988168192-djBY?utm_source=share&utm_medium=member_desktop&rcm=ACoAACnlDeIBNAmrm1dfSEt62mCOeOPvBMOiuFk)**  
*(LinkedIn Technical Post — March 2026)*  
Stress-tested the Sigmoid-NLARX NMPC framework against chaotic 50–120% gain perturbations simulating real-world pressure leakage and effort spikes. NMPC held 3.721 mm RMSE while PID cascaded into failure. Identified the 110% stable boundary and selected the 400s compute baseline as the optimal deployment candidate — nearly 4x more efficient than the max-precision configuration. An extension of the GNC Robotics Framework (Report 03.5), independent of ongoing publications.

---
## Projects

### [PersonalFinance — Budget Aggregator](https://github.com/BryanLukehartYun/PersonalFinance-BudgetAggregator)
A fully local, privacy-first budget aggregator built in Python. Ingests CSV exports from multiple banks and runs every transaction through a 5-layer categorization pipeline — exact lookup, fuzzy matching (RapidFuzz), and semantic similarity via a local offline BGE encoder — outputting a single annotated master CSV. No data leaves the local machine. Built with `uv` for deterministic dependency management across macOS and Linux.

---

## Research

**Thesis:** Stable Open-Loop Modelling of McKibben Muscle with Tunable Slider  
**Institution:** Rochester Institute of Technology — BioSEL Lab  
**Timeframe**: January 2023 - December 2025   
**Supervisor:** Dr. Kathleen Lamkin-Kennard  
**Status:** Under embargo pending publications in **IEEE T-RO, IJRR, and Data in Brief**  
**Archive:** [RIT Digital Commons](https://repository.rit.edu)   

> Note: I'm still involved with the BioSEL lab on assistance and operating in a "Client" capacity while Publications are ongoing. This is projected to end late ~2026 but is not listed with the timeframe

**REU:** Harvard University — **Whitesides Research Group** (2019)    
Fabrication and validation of kirigami actuators. Direct academic lineage to the foundational soft robotics research that motivates this work.  

[REU Profile Link](https://sites.google.com/g.harvard.edu/reu-participant-profiles/2019)

> Note: In no such capacity or any statements do I claim to be part of his umbrella, this is just a informal showcase showing where the origins of my experience originated. 
---

## Contact

| Inquiry | Contact |
|---|---|
| Recruitment & Professional | bryan.lukehartyun@gmail.com |
| Research Collaboration | wwy6929@rit.edu |
| Technical & Repository | Open a GitHub Issue |
