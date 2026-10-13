# Hi there, I'm Pablo Orellana Chornyak 👋
### Computational Physicist & Scientific Software Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com)
[![Email](https://img.shields.io/badge/Email-Contact_Me-D14836?style=for-the-badge&logo=gmail)](mailto:pabloore@correo.ugr.es)
[![Degree](https://img.shields.io/badge/B.Sc._Physics-Universidad_de_Granada-E03A3E?style=for-the-badge)](https://www.ugr.es/)

I am a Physicist specializing in **Computational Physics**, **High-Performance Computing (HPC)**, and **Astrophysics**. My work focuses on solving non-linear inverse problems, numerical partial differential equations, orbital optimization, and multi-body gravitational simulations.

---

## 🛠️ Technical Stack & Skills

- **Languages**: Python 3, Fortran (95/2003), C/C++, Bash, LaTeX
- **Scientific Computing & Libraries**: NumPy, SciPy, Astropy, SunPy, Pandas, Matplotlib, Manim
- **High-Performance Computing (HPC)**: OpenMP, F2PY (Fortran-Python C-API bindings), Multiprocessing, Vectorization
- **Domains**: Solar Spectropolarimetry, Celestial Mechanics & Astrodynamics, Quantum Dynamics, Numerical PDEs, Evolutionary Optimization (Genetic Algorithms)
- **Developer Tools**: Git, GitHub, Linux / Unix, Makefiles

---

## 🚀 Featured Portfolio Projects

### ☀️ [Solar Spectropolarimetry & Optical Deconvolution](https://github.com/REPLACE_WITH_USERNAME/solar-weak-field-deconvolution)
> **Bachelor's Thesis (TFG) in Physics** in collaboration with the **Instituto de Astrofísica de Andalucía (IAA-CSIC)**.
- **Problem**: Mitigating diffraction and optical aberrations (PSF) in stratospheric solar observations from the **SUNRISE III / TuMag** balloon mission.
- **Methods**: Solves the inverse problem for Weak Field Approximation (WFA) of Stokes $V$ by developing a **spatially coupled forward model** (van Noort framework) with a matrix-free **Conjugate Gradient** solver ($\mathcal{O}(N)$ memory).
- **Highlights**: Avoids catastrophic noise amplification on bipolar polarimetric signals; validated on synthetic solar convection models and observational TuMag FITS data.
- **Tech**: `Python`, `Astropy`, `SciPy`, `SunPy`, `NumPy`, `LaTeX`

---

### 🛰️ [Interplanetary Trajectory Optimization (Earth-to-Mars Transfer)](https://github.com/REPLACE_WITH_USERNAME/interplanetary-trajectory-optimization)
> **Astrodynamics & Multi-Body Evolutionary Optimization**
- **Problem**: Finding fuel-optimal transfer orbits from Earth to Mars in a restricted multi-body gravitational environment (Sun, Earth, Moon, Mars).
- **Methods**: Hybrid architecture coupling a high-performance **Fortran 95 Runge-Kutta 4 (RK4)** numerical integrator with Python **Genetic Algorithms (GA)** via `f2py` and distributed `multiprocessing`.
- **Highlights**: Discovers lunar gravity-assist trajectories and optimal orbital injection windows; generates 2D/3D trajectory animations.
- **Tech**: `Fortran 95`, `Python`, `F2PY`, `Multiprocessing`, `NumPy`, `Matplotlib`

---

### 🪐 [Real Solar System (RSS): N-Body Gravitational Dynamics](https://github.com/REPLACE_WITH_USERNAME/solar-system-nbody-simulation)
> **Symplectic Celestial Mechanics & Molecular Dynamics Analogy**
- **Problem**: Simulating the gravitational interaction of the 9 principal Solar System bodies over astronomical timescales without secular energy drift.
- **Methods**: Symplectic **Velocity-Verlet algorithm** in a non-dimensionalized coordinate system ($r'=r/\text{AU}$, $m'=m/M_\odot$, $GM_\odot \to 1$).
- **Highlights**: Verified against NASA/JPL observational ephemerides; simulates Mercury perihelion advance and planetary orbital resonances; animated in 3D using **Manim**.
- **Tech**: `Fortran 95`, `Python`, `Manim`, `Matplotlib`, `Make`

---

### ⚛️ [Time-Dependent Schrödinger Equation Solver (TDSE 1D)](https://github.com/REPLACE_WITH_USERNAME/quantum-schrodinger-solver)
> **Computational Quantum Mechanics & Numerical PDEs**
- **Problem**: Simulating wave packet evolution, quantum tunneling, and harmonic potential oscillations.
- **Methods**: Implicit **Crank-Nicolson** finite-difference scheme (Cayley transform) ensuring exact norm conservation ($\int |\Phi|^2 dx = 1$) and unconditional stability; tridiagonal system inverted via the **Thomas algorithm** in $\mathcal{O}(N)$ time.
- **Highlights**: Parallelized multi-grid parameter studies using **OpenMP**; extracts quantum revival periods and autocorrelation functions $C(t) = \langle \Phi(0)|\Phi(t)\rangle$.
- **Tech**: `Fortran 95`, `OpenMP`, `Python`, `SciPy`, `Matplotlib`

---

## 🎓 Education & Background

- **B.Sc. in Physics (Grado en Física)** — Universidad de Granada (UGR), Spain
- **Research Collaboration**: Departamento de Física Solar, Instituto de Astrofísica de Andalucía (IAA-CSIC)

---

## 📫 Get in Touch

- **GitHub**: [github.com/REPLACE_WITH_USERNAME](https://github.com/REPLACE_WITH_USERNAME)
- **Email**: [pabloore@correo.ugr.es](mailto:pabloore@correo.ugr.es)

