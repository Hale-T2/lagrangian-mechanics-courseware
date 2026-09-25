
HALE TÜRELİ AP Physics C Mech & EM 2026 Project
Robert College Istanbul TURKEY

# Lagrangian Mechanics for AP Physics C: Courseware & Analytical Framework

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

An educational repository and analytical framework designed for **AP Physics C (Mechanics and Electromagnetism)** students and educators. This project bridges standard Calculus BC concepts and Newtonian vector mechanics with the scalar energy framework of **Lagrangian Mechanics**—completely bypassing messy 3D vector constraint forces while maintaining mathematical rigor without linear algebra or Hamiltonian formalism.

---

## 📌 Project Overview & Key Highlights

This courseware transitions students from Newtonian vector mechanics (\\(\mathbf{F}=m\mathbf{a}\\)) to Lagrangian scalar mechanics (\\(L = T - V\\)) through intuitive physics models, symbolic math derivations, and interactive Jupyter notebooks:

* **3D Vectors vs. Scalar Energies:** Move beyond free-body diagrams and shifting constraint forces (normal forces, rope tension) to single scalar energy functions.
* **Mechanical Systems:** Derive non-linear pendulum equations and harmonic oscillations using polar generalized coordinates (\\(q_i\\)).
* **Electromagnetism & Velocity-Dependent Potentials:** Derive the Lorentz force law \\(\mathbf{F} = q(\mathbf{E} + \mathbf{v} \times \mathbf{B})\\) using the magnetic vector potential \\(\mathbf{A}\\) and the multivariable chain rule.
* **Kinematic vs. Canonical Momentum:** Explore why conserved momentum in a magnetic field includes field potential momentum (\\(\mathbf{p} = m\mathbf{v} + q\mathbf{A}\\)).
* **Non-Conservative Drag & Friction:** Model velocity-dependent air resistance (\\(F_f = -kv\\)) using **Rayleigh's Dissipation Function** \\(D = \frac{1}{2} k v^2\\).

---

## 📂 Repository Structure

```text
lagrangian-mechanics-courseware/
├── README.md                                          # Project overview and documentation
├── requirements.txt                                   # Python dependencies (NumPy, SciPy, Matplotlib, SymPy)
└── notebooks/
    ├── 01_Newton_vs_Lagrange_Foundations.ipynb        # Philosophical & mathematical foundations
    ├── 02_Mechanical_Systems_Oscillators_Pendulums.ipynb # Pendulum dynamics & small-angle limits
    ├── 03_Air_Resistance_Rayleigh_Dissipation.ipynb   # Viscous drag & damped projectile trajectories
    └── 04_Electromagnetism_Lorentz_Force.ipynb        # Velocity potentials & 3D cyclotron orbits
```

---

## 📚 Core Analytical Modules

### 1. Philosophical & Mathematical Foundations
* **Principle of Stationary Action:** $\delta S = \delta \int L \, dt = 0$.
* **Euler-Lagrange Equation:** 

$$\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{q}_i}\right) - \frac{\partial L}{\partial q_i} = 0$$

* **Constraint Elimination:** Explains how generalized coordinates $q_i$ automatically account for holonomic constraints, eliminating unknown reaction forces.

### 2. Mechanical Systems & Pendulum Dynamics
* **Lagrangian Setup:** $L = T - V = \frac{1}{2} m l^2 \dot{\theta}^2 + m g l \cos\theta$.
* **Equation of Motion:** $m l^2 \ddot{\theta} + m g l \sin\theta = 0$.
* **Numerical Analysis:** Solves exact non-linear trajectories for large initial angles ($\theta_0 = 120^\circ$) and compares against the small-angle approximation ($\sin\theta \approx \theta$).

### 3. Air Resistance via Rayleigh Dissipation
* **Dissipation Function:** $D = \frac{1}{2} k (\dot{x}^2 + \dot{y}^2 + \dot{z}^2)$.
* **Modified Euler-Lagrange Equation:**

$$\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{q}_k}\right) - \frac{\partial L}{\partial q_k} + \frac{\partial D}{\partial \dot{q}_k} = 0$$

* **Damped Trajectories:** Derives and simulates $m\ddot{x} + k\dot{x} = 0$ and $m\ddot{z} + k\dot{z} + mg = 0$ for realistic atmospheric projectiles.

### 4. Electromagnetism & The Lorentz Force
* **Generalized Velocity-Dependent Potential:** $V = q\Phi - q\mathbf{v}\cdot\mathbf{A}$.
* **Lagrangian for a Charged Particle:** $L = \frac{1}{2} m v^2 - q\Phi + q\mathbf{v}\cdot\mathbf{A}$.
* **Canonical Momentum:** $\mathbf{p} = \frac{\partial L}{\partial \mathbf{v}} = m\mathbf{v} + q\mathbf{A}$.
* **Multivariable Chain Rule Expansion:** Demonstrates how $\frac{d\mathbf{A}}{dt} = \frac{\partial \mathbf{A}}{\partial t} + (\mathbf{v}\cdot\nabla)\mathbf{A}$ and spatial partial derivatives cleanly assemble the cross-product $q(\mathbf{v} \times \mathbf{B})$.

---

## 🚀 Quick Start Guide

### Prerequisites
* Python 3.10 or higher
* Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Hale-T2/lagrangian-mechanics-courseware.git
   cd lagrangian-mechanics-courseware
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebooks:**
   ```bash
   jupyter notebook
   ```

---

## 🤝 Syllabus Mapping for AP Physics C

| AP Physics C Topic | Newtonian Approach | Lagrangian Approach | Notebook Module |
| :--- | :--- | :--- | :--- |
| **Particle Dynamics** | Free-Body Diagrams, $\mathbf{F}=m\mathbf{a}$ | Scalar Energies ($L=T-V$) | Module 01 |
| **Rotational & Pendulum Motion** | Torque $\mathbf{\tau}=I\mathbf{\alpha}$, Tension $\mathbf{T}$ | Generalized Angle $\theta$, Euler-Lagrange | Module 02 |
| **Non-Conservative Drag** | Differential Drag Force $\mathbf{F}_d = -k\mathbf{v}$ | Rayleigh Dissipation Function $D$ | Module 03 |
| **Magnetic Forces** | Lorentz Force $\mathbf{F}=q(\mathbf{v}\times\mathbf{B})$ | Vector Potential $\mathbf{A}$, Canonical Momentum $\mathbf{p}$ | Module 04 |

---

## 📜 License
This project is open-source under the [MIT License](LICENSE).
```

***

### How to update it on GitHub:
1. Go to your repository at `https://github.com/Hale-T2/lagrangian-mechanics-courseware`.
2. Click on `README.md`, then click the pencil icon (**Edit this file**) in the top right corner.
3. Paste the code block above into the editor.
4. Click **Commit changes...** at the top right.
