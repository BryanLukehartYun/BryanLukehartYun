# Bryan Lukehart-Yun

**M.S. Mechanical Engineering — Rochester Institute of Technology (2025)**  
*Dynamic Systems, Nonlinear SysID, State Estimation & Soft Actuators*  
[Email](mailto:bryan.lukehartyun@gmail.com) | [Publications](#publications)

---

I build experimental testbeds, open datasets, and estimation/control pipelines for hysteretic and nonlinear physical systems. My work centers on high-rate empirical system identification, derivative-free state estimation under severe non-differentiable dynamics, and physical soft robotics characterization.

Previously conducted research at **NRL** (hexapod C++ kinematic constraints), **ARL** (piezoelectric MEMS batch V&V), and **Harvard** (**Whitesides Research Group**, kirigami actuators). Currently preparing doctoral applications in mechanical engineering and robotics.

### Core Technical Focus
* **Nonlinear SysID & Hysteresis Modeling:** Characterized soft actuator dynamics across 24 operating regimes, cutting open-loop hysteretic drift by 91%.
* **State Estimation & Control:** Formulated UKF and NMPC pipelines to overcome Jacobian-spike singularities inherent to EKF on non-differentiable soft actuators.
* **Open Science & Data Infrastructure:** Engineered a 50M+ sample high-rate time-series testing pipeline (100/200 Hz), release toolchains, and hardware CAD test rigs.

---

## Featured Work

### [Empirical-Modeling-and-Data-Driven-Control-for-Nonlinear-Soft-Actuators](https://github.com/BryanLukehartYun/Empirical-Modeling-and-Data-Driven-Control-of-Nonlinear-Soft-Actuators)
Framework combining nonlinear SysID (NLARX), derivative-free state estimation (UKF), and NMPC trajectory tracking for pneumatic artificial muscles. Features an open-source Python processing stack (10–12× speedup over legacy MATLAB) supporting 11 interchangeable filtering methods via YAML configs and multi-core batch execution. 

### [Applied-Dynamics-and-Controls](https://github.com/BryanLukehartYun/Applied-dynamics-and-controls)
Dynamics, estimation, and mission design testbeds: 6-DOF nonlinear flight truth models, quaternion UKF attitude estimation under randomized disturbance noise, and interplanetary trajectory optimization with symbolic $\Delta V$ derivations.

---

## Publications & Preprints

* **Lukehart-Yun, B.** et al., *"A Large-Scale Time-Series Dataset for McKibben-Style Pneumatic Artificial Muscles and Soft Robotics Research,"* Data in Brief, 2026. *Under review.* [doi:10.5281/zenodo.23066619]
* **Lukehart-Yun, B.** and Lamkin-Kennard, K., *"Stable Open-Loop Modelling of McKibben Muscle with Tunable Slider,"* *In preparation for IEEE Robotics and Automation Letters (RA-L)*, 2026.

---

## Environment & Tooling

* **Computing & Controls:** Python (`uv`, NumPy, SciPy, pandas, scikit-learn, PyWavelets), C++, MATLAB / Simulink
* **Lab & DAQ:** High-rate data acquisition, optical/load cell instrumentation, ASTM materials testing, FDM/SLA rapid prototyping
* **Infrastructure & Homelab:** Tailscale mesh network, self-hosted Forgejo Git server, Linux (CachyOS/Arch), macOS
* **Workflow:** Neovim / Neovide, VimTeX + Zathura, plain-text task tracking, DOOM Emacs with **EVIL**
