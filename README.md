# Hi there, I'm Pablo Orellana Chornyak 👋
### Space Science & Technology Student | Computational Physicist

[![Master](https://img.shields.io/badge/M.Sc._Space_Science_%26_Technology-Univ._de_Alcalá-990000?style=for-the-badge)](https://www.uah.es/)
[![Degree](https://img.shields.io/badge/B.Sc._Physics-Universidad_de_Granada-E03A3E?style=for-the-badge)](https://www.ugr.es/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-p--orellana-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/p-orellana)
[![Email](https://img.shields.io/badge/Email-pablo.orellana.physics%40gmail.com-D14836?style=for-the-badge&logo=gmail)](mailto:pablo.orellana.physics@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-porellanaphysics-181717?style=for-the-badge&logo=github)](https://github.com/porellanaphysics)

---

### 🚀 Sobre mí / About Me

> **Graduado en Física por la Universidad de Granada (UGR)** con experiencia en física computacional y análisis de datos astrofísicos. Actualmente cursando el **Máster en Ciencias y Tecnologías desde el Espacio en la Universidad de Alcalá (UAH, Alcalá de Henares)**, con especial interés en análisis de misiones espaciales, mecánica orbital, simulación de trayectorias, transferencia radiativa e integración numérica de ecuaciones diferenciales.

I am a Physicist specializing in **Space Sciences & Technology**, **Astrodynamics**, and **Computational Physics**. My work focuses on solving non-linear inverse problems in astrophysics, interplanetary trajectory optimization, N-body gravitational simulations, and numerical partial differential equations.

---

## 🛠️ Competencias Técnicas / Technical Stack

- **Lenguajes de programación**: Python (NumPy, SciPy, Matplotlib), C++, Fortran (95/2003), Bash, LaTeX
- **Métodos Numéricos & Computación Científica**: Integración numérica de EDOs/EDPs (Runge-Kutta 4, Verlet, Crank-Nicolson), algoritmos de deconvolución óptica (Richardson-Lucy, gradiente conjugado), análisis espectropolarimétrico, ajuste y análisis de series temporales
- **Mecánica Orbital & Astrodinámica**: Dinámica de $N$ cuerpos, transferencias orbitales (Hohmann y multi-cuerpo asistido), optimización evolutiva mediante Algoritmos Genéticos (GA)
- **Librerías & Herramientas Astrofísicas**: Astropy, SunPy, Photutils, Manim, OpenMP, F2PY, Git / GitHub, Linux

---

## 🌟 Proyectos Destacados / Featured Projects

### ☀️ [Solar Spectropolarimetry & Optical Deconvolution](https://github.com/porellanaphysics/solar-weak-field-deconvolution)
> **Trabajo de Fin de Grado (Calificación: 9,4 / 10)** — En colaboración con el **Instituto de Astrofísica de Andalucía (IAA-CSIC)**.
- **Problema**: Mitigación de la difracción y aberraciones ópticas (PSF) en observaciones estratosféricas de alta resolución del telescopio **SUNRISE III** (instrumento **TuMag**).
- **Metodología**: Resolución del problema inverso para la Aproximación de Campo Débil (WFA) sobre Stokes $V$ mediante un **modelado directo acoplado espacialmente** (marco de van Noort) con optimizador de **Gradiente Conjugado *matrix-free*** ($\mathcal{O}(N)$ en memoria).
- **Resultados**: Evita la amplificación incontrolada de ruido en la señal bipolar de Stokes $V$; probado en datos sintéticos solares y observaciones reales FITS de gránulos del Sol en calma.
- **Stack**: `Python`, `Astropy`, `SciPy`, `SunPy`, `NumPy`, `LaTeX`

---

### 🛰️ [Interplanetary Trajectory Optimization (Earth-to-Mars Transfer)](https://github.com/porellanaphysics/interplanetary-trajectory-optimization)
> **Astrodinámica & Optimización Evolutiva de Múltiples Cuerpos** (Física Computacional, UGR).
- **Problema**: Cálculo y optimización de trayectorias de transferencia orbital Tierra-Marte en un entorno gravitatorio restringido multi-cuerpo (Sol, Tierra, Luna, Marte).
- **Metodología**: Integrador numérico **Runge-Kutta 4 (RK4)** acoplado a un motor de **Algoritmos Genéticos (GA)** en Python con multiprocesamiento paralelo para explorar el espacio de parámetros $(\theta_0, v_0, \Delta \vec{v}, t_{\mathrm{burn}})$.
- **Resultados**: Obtención automática de ventanas de eyección, maniobras de asistencia gravitatoria lunar y aproximaciones de mínima energía; animaciones de trayectoria en MP4.
- **Stack**: `Fortran 95`, `Python`, `F2PY`, `Multiprocessing`, `NumPy`, `Matplotlib`

---

### 🪐 [Real Solar System (RSS): N-Body Gravitational Dynamics](https://github.com/porellanaphysics/solar-system-nbody-simulation)
> **Mecánica Celeste Simpléctica & Simulación Gravitacional**
- **Problema**: Simulación gravitacional newtoniana del Sistema Solar completo ($N=9$ cuerpos) a lo largo de escalas temporales astronómicas sin deriva secular de energía.
- **Metodología**: Integrador simpléctico **Velocity-Verlet** bajo un sistema adimensionalizado ($r'=r/\text{UA}, m'=m/M_\odot, t'=t/\mu \implies GM_\odot = 1$).
- **Resultados**: Verificación con efemérides observacionales reales de NASA/JPL; cálculo de periodos orbitales y avance del perihelio de Mercurio; renderizado cinemático 3D en **Manim**.
- **Stack**: `Fortran 95`, `Python`, `Manim`, `Matplotlib`, `Make`

---

### ⚛️ [Time-Dependent Schrödinger Equation Solver (TDSE 1D)](https://github.com/porellanaphysics/quantum-schrodinger-solver)
> **Mecánica Cuántica Computacional & EDPs Numéricas**
- **Problema**: Simulación de la evolución de paquetes de ondas cuánticos, osciladores armónicos y dispersión/efecto túnel en barreras de potencial.
- **Metodología**: Esquema implícito unitario de **Crank-Nicolson** (transformada de Cayley) garantizando conservación estricta de la norma ($\int |\Phi|^2 dx = 1$); inversión tridiagonal en tiempo lineal $\mathcal{O}(N)$ mediante el **algoritmo de Thomas**.
- **Resultados**: Barridos multiparamétricos paralelizados en CPU multi-core mediante **OpenMP**; extracción de periodos armónicos mediante la función de autocorrelación $C(t) = \langle \Phi(0)|\Phi(t)\rangle$.
- **Stack**: `Fortran 95`, `OpenMP`, `Python`, `SciPy`, `Matplotlib`

---

## 🎓 Formación Académica / Education

- **Máster Universitario en Ciencias y Tecnologías desde el Espacio** — Universidad de Alcalá (UAH, Alcalá de Henares) | *2026 – 2027 (En curso)*
  - *Módulos clave*: Astrofísica Espacial, Interacción Sol-Tierra: Meteorología Espacial, Exploración del Sistema Solar, Software de Control en Tiempo Real para Sistemas Espaciales, Ingeniería y Gestión de Proyectos Espaciales, IA en Sistemas de Control Autónomo.
- **Grado en Física** — Universidad de Granada (UGR) | *2022 – 2026 (Completado)*
  - *Asignaturas relevantes*: Métodos Numéricos, Programación, Física Computacional, Mecánica, Mecánica Cuántica, Astrofísica.
  - *Trabajo de Fin de Grado*: Calificación **9,4 / 10** en colaboración con el IAA-CSIC.

---

## 📬 Contacto / Contact

- **Email**: [pablo.orellana.physics@gmail.com](mailto:pablo.orellana.physics@gmail.com)
- **LinkedIn**: [linkedin.com/in/p-orellana](https://linkedin.com/in/p-orellana)
- **GitHub**: [github.com/porellanaphysics](https://github.com/porellanaphysics)
- **Ubicación**: Alcalá de Henares (Madrid), España

