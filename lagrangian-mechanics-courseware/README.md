# Lagrangian Mechanics Courseware & GitHub Repository

A comprehensive courseware repository designed for **AP Physics C (Mechanics & Electromagnetism)** and **Calculus BC** students studying analytical mechanics.

---

## 📚 Repository Overview

This repository provides interactive Jupyter Notebooks, mathematical derivations, SymPy symbolic verifications, and SciPy numerical simulations comparing **Newtonian Mechanics** and **Lagrangian Mechanics**.

### 📁 Structure

```text
lagrangian-mechanics-courseware/
├── README.md
├── requirements.txt
└── notebooks/
    ├── 01_Newton_vs_Lagrange_Foundations.ipynb
    ├── 02_Mechanical_Systems_Oscillators_and_Pendulums.ipynb
    ├── 03_Air_Resistance_Rayleigh_Dissipation.ipynb
    └── 04_Electromagnetism_Lorentz_Force.ipynb
```

---

## 📖 Notebook Summaries

1. **`01_Newton_vs_Lagrange_Foundations.ipynb`**
   - Conceptual comparison between vector force mechanics $\mathbf{F}=m\mathbf{a}$ and scalar energy mechanics $L=T-V$.
   - Derivation of the Euler-Lagrange Equation from the Principle of Stationary Action $\delta S = 0$.
   - How generalized coordinates $q_i$ eliminate unknown constraint forces.

2. **`02_Mechanical_Systems_Oscillators_and_Pendulums.ipynb`**
   - Simple Harmonic Oscillator and Pendulum derivations in polar coordinates.
   - SymPy derivation of non-linear pendulum differential equation $\ddot{\theta} + \frac{g}{l}\sin\theta = 0$.
   - SciPy numerical integration comparing exact non-linear motion vs. small-angle approximation ($\sin\theta \approx \theta$).

3. **`03_Air_Resistance_Rayleigh_Dissipation.ipynb`**
   - Extending Lagrangian mechanics to non-conservative forces.
   - Formulation of **Rayleigh's Dissipation Function** $D = \frac{1}{2}k(\dot{x}^2 + \dot{y}^2 + \dot{z}^2)$.
   - Modified Euler-Lagrange equation with dissipation:
     $$\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{q}_k}\right) - \frac{\partial L}{\partial q_k} + \frac{\partial D}{\partial \dot{q}_k} = 0$$
   - Numerical simulation of 2D projectile trajectories comparing vacuum vs. viscous drag.

4. **`04_Electromagnetism_Lorentz_Force.ipynb`**
   - Velocity-dependent potential $V = q\Phi - q\mathbf{v}\cdot\mathbf{A}$ and Electromagnetic Lagrangian $L = \frac{1}{2}m v^2 - q\Phi + q\mathbf{v}\cdot\mathbf{A}$.
   - **Canonical Momentum** $\mathbf{p} = m\mathbf{v} + q\mathbf{A}$ vs. Kinematic Momentum $\mathbf{\pi} = m\mathbf{v}$.
   - Multivariable chain rule expansion deriving the Lorentz force $m\mathbf{a} = q(\mathbf{E} + \mathbf{v}\times\mathbf{B})$.
   - 3D numerical simulation of cyclotron helical trajectories in EM fields.

---

## 🚀 Installation & Running

```bash
git clone https://github.com/your-username/lagrangian-mechanics-courseware.git
cd lagrangian-mechanics-courseware
pip install -r requirements.txt
jupyter notebook
```

---

## 🎓 AP Physics C & Calculus BC Syllabus Alignment

- **Calculus BC**: Partial derivatives, multivariable chain rule, Taylor series expansions, non-linear ODE numerical solving.
- **Physics C Mechanics**: Oscillations, non-conservative drag forces, energy conservation, generalized forces.
- **Physics C E&M**: Magnetic vector potential $\mathbf{A}$, Lorentz force $\mathbf{F} = q(\mathbf{E} + \mathbf{v}\times\mathbf{B})$, canonical momentum.
