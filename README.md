# Computational Fluid Dynamics (CFD) Analysis: Airfoil & Nozzle

> **Academic Laboratory Activities — Politecnico di Milano**  
> Course: *Computational Fluid Dynamics - Fundamentals* (A.Y. 2024–2025)
> **Authors:** Simone Falsitta, Antonino Luongo, Davide Monaci
> **Supervisors:** Prof. Giacomo Bruno Azzurro Persico, Prof. Gianluca Montenegro

---

## Project Overview
This repository contains comprehensive CFD simulation projects performed using **OpenFOAM**. The work is divided into two primary fluid dynamics exercises: external flow around an airfoil and internal flow through a converging nozzle.

---

## Exercise 1: Airfoil Analysis (NACA 4412)
* **Objective:** External incompressible turbulent flow analysis around a standard NACA 4412 airfoil at zero angle of attack ($\alpha = 0^\circ$) and $V_{in} = 20\text{ m/s}$.
* **Turbulence Models Explored:**
  * **$k-\epsilon$ Model:** Evaluated with wall functions across coarse, intermediate, and fine structured C-grid meshes.
  * **Spalart-Allmaras (SA) Model:** Analyzed both with wall functions and in a wall-resolving setup without wall functions ($y^+ \le 1$) using a refined 10-block topology.
* **Key Findings:** Detailed evaluations of aerodynamic coefficients ($C_L, C_D, C_m$), pressure and skin friction distributions, velocity wakes, and thorough grid independence studies.

---

## 🌬️ Exercise 2: Nozzle Analysis
* **Objective:** Internal flow simulation through a 2D converging nozzle connecting two rectangular channels[cite: 159].
* **Flow Regimes & Models:**
  * **Laminar Flow:** Low-accuracy to high-accuracy mesh refinements ($1200 \times 120$ cells) tracking mass conservation and velocity reduction coefficients.
  * **Turbulent Flow with Wall Functions:** Implementation of the $k-\epsilon$ model with precise $y^+$ wall constraints ($y^+ > 30$).
  * **Turbulent Flow without Wall Functions:** Wall-resolving $k-\omega \text{ SST}$ model implementation ensuring strict boundary layer adherence ($y^+ < 1$).
* **Key Findings:** Cross-sectional pressure drops, total-to-static pressure distributions, wall shear stress peaks, and turbulence mixing comparisons.

---
## Project Team & Academic Context

## Group Members
* **Simone Falsitta**
* **Antonino Luongo** 
* **Davide Monaci** 

**Politecnico di Milano 1863**  
*School of Industrial and Information Engineering — M.Sc. in Mechanical Engineering* (A.Y. 2024–2025)  
**Course**: *Advanced Dynamics of Mechanical Systems*
