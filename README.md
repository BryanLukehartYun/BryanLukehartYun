# Bryan Lukehart-Yun

**M.S. Mechanical Engineering — Rochester Institute of Technology (2025)**  
**Focus: Guidance, Navigation, and Control (Targeting for Roles) | Nonlinear Dynamics with Modeling | State Estimation | Robotics**

---

## About Me

I'm a recent M.S. graduate in Mechanical Engineering (RIT, Dec 2025) with research focus on nonlinear actuator dynamics and Controls system. My work sits at the intersection of classical control theory and modern nonlinear methods—from 6-DOF fixed-wing simulations to NMPC-driven soft actuator control.

Currently preparing **three manuscripts for submission** to IEEE Transactions on Robotics, International Journal of Robotics Research, and Data in Brief on nonlinear soft actuator control. Expected submission: Q2 2026; projected publication: Q4 2026. 

I am also currently in the process of releasing full framework regarding thesis when both T-RO and Data in Brief are submitted. 

**Independent research contributions (post-thesis, Dec 2025 onward):**
* Identified and quantified the "Jacobian spike" failure mode in EKF/CKF when applied to soft actuators with non-differentiable hysteresis
* Developed UKF-based derivative-free estimation strategy, eliminating −7.5 mm tracking bias and achieving 99.9% state estimation fidelity (Python)
* Simulated NMPC + UKF combo achieving 1–6 mm RMSE tracking under 33–140% chaotic environmental perturbations based on a anonymized slice of data from research. 

I bring classical aerospace GNC knowledge (based on graduate coursework) such as 6-DOF nonlinear truth models, linearization audits, modal stability analysis, and the full V&V workflow that flight control development requires in theory. 

Prior to graduate research, I've worked across the federal research and industry pipeline: Naval Research Laboratory (robotics integration and multiaxial test systems), Army Research Laboratory (MEMS fabrication and sensor V&V), Harvard under **Whitesides Research Group** (soft actuator fabrication), and DOW Inc. (materials testing and Python-based measurement automation).

---

## Domain-Agnostic GNC: From Soft Actuators and Co-ops to Aerospace & Robotics

While my recent research derived from my M.S. thesis focuses on soft pneumatic actuators as well as prior works, the core contributions are **universally applicable** across nonlinear control domains. The soft actuator problem is deliberately chosen as a difficult testbed since if these methods solve hysteretic nonlinearity, they transfer to less-constrained systems.

| **Your Work** | **Aerospace Application** | **General Robotics Application** |
|---|---|---|
| **6-DOF Nonlinear Truth Modeling & Linearization Audit** | High-fidelity flight simulators for aircraft/spacecraft transition phases | Full-body physics engines for legged locomotion or multi-joint systems | 
| **Nonlinear plant identification (NLARX)** | Aircraft aerodynamic model ID from flight test data | Actuator dynamics learning; system adaptation to aging/temperature |
| **UKF for state estimation under nonlinear hysteresis** | Aircraft attitude estimation with actuator saturation & sensor bias | Manipulator joint state with friction/backlash; quadrotor localization under IMU drift |
| **Jacobian Proxy Analysis for Estimator Stability** | Formally quantifying when an EKF will fail during high-dynamic flight maneuvers | Proving estimator reliability for highly nonlinear soft-body or bio-inspired robots | 
| **NMPC trajectory tracking with constraints** | Reference flight path tracking under aerodynamic uncertainty | Autonomous vehicle waypoint following; robot arm reaching tasks |
| **Robustness validation via Monte Carlo under chaos** | Flight control under wind gusts + sensor noise + actuator faults | Robot motion under environmental disturbances + wear |
| **Kinematic Constraints & Collision Avoidance (C++)** | Autonomous docking maneuvers or robotic satellite servicing (OSAM-1 for example) | Safety-Critical Motion Planning: Industrial arms in shared workspaces | 
| **Large-scale Signal Processing (15M+ samples)** | Real-time telemetry analysis and flight test data reduction for airframe stress | Big Data Robotics: Processing massive sensor logs for fleet-wide predictive maintenance |  

The technical depth from Federal labs (NRL, ARL) and DOW demonstrates ability to work across materials science, sensor integration, and manufacturing constraints which are all applicable to aerospace/robotics system design.

---

## Technical Stack  

<table align="center">
  <tr>
    <td align="center">
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=BryanLukehartYun&theme=radical" alt="Streak Card" />
    </td>
  </tr>
</table>

  
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=BryanLukehartYun&layout=compact&theme=radical" alt="Top Languages" />
</p> 


| Domain | Tools |
|---|---|
| Primary Language | Python |
| Legacy / Simulation | MATLAB / Simulink |
| Embedded & Robotics | C++ |
| Control Methods | NMPC, PID, State-Space |
| Operating Systems | Linux (Arch, Debian), MacOS, Windows (Work-Related)|
| Git | GitHUB, Forgejo (Fork of Gitea)|
| Estimation | UKF, EKF, CKF |
| System ID | NLARX (Sigmoid, Wavelet, idTreePartition), Mathematical Modeling, Model Selection |
| Statistical Analysis | GMM (AIC / BIC), Multimodality Testing (Hartigan’s Dip, Silverman’s Test, Excess Mass)
| Fabrication | FDM, SLA, Soft Robotics, CAD |
| Standards | ASTM C642, E2178, E2357, D143 |

> Self-hosted Forgejo + Bookstack on homelab (Tailscale) for private research versioning, documentation, and technical projects. 

> Also making use of dedicated and secondary hardwares to run Modeling & Simulation, Computational, and Machine Learning (based on Brunton & Kutz's [DATA DRIVEN SCIENCE & ENGINEERING: Machine Learning, Dynamical Systems and Control](https://databookuw.com/)).

---

## Featured Repositories

### [Empirical-Modeling-and-Control-for-Nonlinear-Soft-Actuators](https://github.com/BryanLukehartYun/Empirical-Modeling-and-Data-Driven-Control-of-Nonlinear-Soft-Actuators) - [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18737435.svg)](https://doi.org/10.5281/zenodo.18737435)
Full framework for Pneumatic Artificial Muscles that pertains to Empirical Modeling and Controls. Currently features NLARX system identification, UKF state estimation validated via Monte Carlo simulation, and NMPC achieving a 75.6% reduction in tracking error vs. baseline PID derived from legacy MATLAB stack and extended. Recently finished porting to Python as of mid April 2026. **Derived from M.S. thesis research at RIT BioSEL Lab.**

### [Applied-Dynamics-and-Controls](https://github.com/BryanLukehartYun/Applied-dynamics-and-controls)
Aerospace GNC portfolio spanning flight dynamics, state estimation, and 
interplanetary mission design. Modules: 6-DOF nonlinear truth model with 
full modal stability analysis; satellite quaternion UKF with Monte Carlo 
validation; and constrained Earth-to-Saturn trajectory optimization with 
symbolically-derived delta-V cost function. Python migration and 
interactive visualization in progress. This repo serves as proof that I can pivot to GNC or aerospace roles in the Aerospace or Defense sector. This is based on the **Graduate courseworks** 
* Flight Dynamics 
* Optimal Design (Course in Optimization techniques both unconstrained and constrained)
* Nonlinear Controls 
* Orbital Mechanics 

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
