# Bryan Lukehart-Yun

**M.S. Mechanical Engineering — Rochester Institute of Technology (2025)**  
**Focus: Guidance, Navigation, and Control | Nonlinear Dynamics | State Estimation | Robotics**

---

## About Me

I'm a recent M.S. graduate in Mechanical Engineering (RIT, Dec 2025) developing control systems for nonlinear soft actuators using classical and modern methods—from 6-DOF simulations to NMPC-driven controllers. Prior to this, I worked across the federal research and industry pipeline: Naval Research Laboratory (robotics integration and multiaxial test systems), Army Research Laboratory (MEMS fabrication and sensor V&V), Harvard under **Whitesides Research Group** (soft actuator fabrication), and DOW Inc. (materials testing and Python-based measurement automation).

Currently preparing **three manuscripts for submission** to IEEE Transactions on Robotics, International Journal of Robotics Research, and Data in Brief on nonlinear soft actuator control. Framework release planned for Q2 2026. 

**Independent research contributions (post-thesis, Dec 2025 onward):**
* Identified and quantified the "Jacobian spike" failure mode in EKF/CKF when applied to soft actuators with non-differentiable hysteresis
* Developed UKF-based derivative-free estimation strategy, eliminating −7.5 mm tracking bias and achieving 99.9% state estimation fidelity (Python)
* Simulated NMPC + UKF combo achieving 1–6 mm RMSE tracking under 33–140% chaotic environmental perturbations 

Federal lab experience (NRL, ARL) plus DOW gives me hands-on expertise in materials science, sensor integration, and manufacturing constraints—all critical for aerospace/robotics design. I also bring classical aerospace GNC expertise from graduate-level coursework in flight dynamics, optimal design, nonlinear controls, and orbital mechanics.

---

## Featured Repositories

### [Empirical-Modeling-and-Data-Driven-Control-for-Nonlinear-Soft-Actuators](https://github.com/BryanLukehartYun/Empirical-Modeling-and-Data-Driven-Control-of-Nonlinear-Soft-Actuators) - [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18737435.svg)](https://doi.org/10.5281/zenodo.18737435)
Soft actuator control framework combining system identification, state estimation, and trajectory optimization. Started as M.S. thesis research and independently extended post-graduation with ongoing contributions. Achieves 75.6% error reduction vs. legacy PID approaches. Recently ported to Python for reproducibility and broader accessibility.

### [Applied-Dynamics-and-Controls](https://github.com/BryanLukehartYun/Applied-dynamics-and-controls)
Aerospace GNC portfolio covering flight dynamics, orbital mechanics, state estimation, and interplanetary mission design. Includes 6-DOF nonlinear truth models, satellite attitude estimation, and Earth-to-Saturn trajectory optimization with symbolic delta-V derivations. Built as graduate-level coursework in flight dynamics, optimal design, and nonlinear controls. Python migration and interactive visualization in progress. 

---

## Technical Stack  

<table align="center">
  <tr>
    <td align="center">
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=BryanLukehartYun&theme=radical" alt="Streak Card" />
    </td>
  </tr>
</table>

> **Note:** Streak stats represent GitHub activity only. Significant development also tracked on self-hosted Forgejo instance for private research and internal projects.

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
| Statistical Analysis | GMM (AIC / BIC), Multimodality Testing (Hartigan's Dip, Silverman's Test, Excess Mass)
| Fabrication | FDM, SLA, Soft Robotics, CAD |
| Standards | ASTM C642, E2178, E2357, D143 |

> Self-hosted Forgejo + Bookstack on homelab (Tailscale) for private research versioning, documentation, and technical projects. 

> Also making use of dedicated and secondary hardwares to run Modeling & Simulation, Computational, and Machine Learning (based on Brunton & Kutz's [DATA DRIVEN SCIENCE & ENGINEERING: Machine Learning, Dynamical Systems and Control](https://databookuw.com/)).

---

## Technical Transferability

The methods developed for soft actuator control are broadly applicable across nonlinear control domains. Below is how core techniques map to aerospace, robotics, and innovation R&D:

| **Your Work** | **Aerospace Application** | **General Robotics Application** | **R&D & Innovation** |
|---|---|---|---|
| **6-DOF Nonlinear Truth Modeling & Linearization Audit** | High-fidelity flight simulators for aircraft/spacecraft transition phases | Full-body physics engines for legged locomotion or multi-joint systems | Enable simulation-driven design of novel soft robot morphologies; accelerate design iteration |
| **Nonlinear plant identification (NLARX)** | Aircraft aerodynamic model ID from flight test data | Actuator dynamics learning; system adaptation to aging/temperature | Rapidly characterize novel materials and actuators without first-principles models; accelerate material discovery |
| **UKF for state estimation under nonlinear hysteresis** | Aircraft attitude estimation with actuator saturation & sensor bias | Manipulator joint state with friction/backlash; quadrotor localization under IMU drift | Real-time feedback control on bleeding-edge actuators with unknown nonlinearities; control systems before full characterization |
| **Jacobian Proxy Analysis for Estimator Stability** | Formally quantifying when an EKF will fail during high-dynamic flight maneuvers | Estimator reliability for nonlinear soft-body or bio-inspired robots | Predict estimator failure modes before prototype testing; de-risk control architectures on novel systems |
| **NMPC trajectory tracking with constraints** | Reference flight path tracking under aerodynamic uncertainty | Autonomous vehicle waypoint following; robot arm reaching tasks | Optimal performance extraction from novel actuators; validate control feasibility before fabrication |
| **Robustness validation via Monte Carlo under chaos** | Flight control under wind gusts + sensor noise + actuator faults | Robot motion under environmental disturbances + wear | Predict prototype performance and edge cases through simulation; reduce expensive physical validation cycles |
| **Kinematic Constraints & Collision Avoidance (C++)** | Autonomous docking maneuvers or robotic satellite servicing (OSAM-1 for example) | Safety-critical motion planning for industrial arms in shared workspaces | Safe exploration of design space for novel morphologies; enable innovation in constrained environments |
| **Large-scale Signal Processing (15M+ samples)** | Real-time telemetry analysis and flight test data reduction for airframe stress | Processing massive sensor logs for fleet-wide predictive maintenance | Data-driven discovery of hidden patterns; identify material properties and failure signatures from large experimental datasets |

---

## Highlights

**[Beyond Stability: NMPC Robustness Under 120% Gain Jitter](https://www.linkedin.com/posts/bryan-lukehart-yun_gnc-robotics-controltheory-activity-7435046592988168192-djBY?utm_source=share&utm_medium=member_desktop&rcm=ACoAACnlDeIBNAmrm1dfSEt62mCOeOPvBMOiuFk)**  
*(LinkedIn Technical Post — March 2026)*  
Stress-tested the Sigmoid-NLARX NMPC framework against chaotic 50–120% gain perturbations simulating real-world pressure leakage and effort spikes. NMPC held 3.721 mm RMSE while PID cascaded into failure. Identified the 110% stable boundary and selected the 400s compute baseline as the optimal deployment candidate — nearly 4x more efficient than the max-precision configuration. An extension of the GNC Robotics Framework (Report 03.5), independent of ongoing publications.

---

## Publications

**In Preparation (2026)**
- Stable Open Loop Modeling on McKibben Muscle with Tunable Slider (Variant based on Thesis) — *IEEE Transactions on Robotics*
- Title TBD — *International Journal of Robotics Research*
- Title TBD — *Data in Brief*

> Titles and scope subject to refinement as submissions progress.

---

## Research

**Thesis:** Stable Open-Loop Modelling of McKibben Muscle with Tunable Slider  
**Institution:** Rochester Institute of Technology — BioSEL Lab  
**Timeframe**: January 2023 - December 2025   
**Supervisor:** Dr. Kathleen Lamkin-Kennard  
**Status:** Under embargo pending publications in **IEEE T-RO, IJRR, and Data in Brief**  
**Archive:** [RIT Digital Commons](https://repository.rit.edu)   

> Note: Currently supporting BioSEL Lab through 2026 while publications are in progress.

**REU:** Harvard University — **Whitesides Research Group** (2019)    
Fabrication and validation of kirigami actuators. Direct academic lineage to the foundational soft robotics research that motivates this work.  

[REU Profile Link](https://sites.google.com/g.harvard.edu/reu-participant-profiles/2019)

---

## Projects

### [PersonalFinance — Budget Aggregator](https://github.com/BryanLukehartYun/PersonalFinance-BudgetAggregator)
A fully local, privacy-first budget aggregator built in Python. Ingests CSV exports from multiple banks and runs every transaction through a 5-layer categorization pipeline — exact lookup, fuzzy matching (RapidFuzz), and semantic similarity via a local offline BGE encoder — outputting a single annotated master CSV. No data leaves the local machine. Built with `uv` for deterministic dependency management across macOS and Linux.

---

## Contact

| Inquiry | Contact |
|---|---|
| Recruitment & Professional | bryan.lukehartyun@gmail.com |
| Research Collaboration | wwy6929@rit.edu |
| Technical & Repository | Open a GitHub Issue |
