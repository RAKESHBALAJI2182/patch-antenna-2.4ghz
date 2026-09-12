# Microstrip Patch Antenna Design (Line / Inset-Fed) - 2.4 GHz

Design and full-wave electromagnetic simulation of an inset line-fed microstrip patch antenna targeting the **2.4 GHz ISM band** using **CST Studio Suite**.

---

## 📡 Antenna Geometry & 3D Structure

The microstrip patch antenna is fabricated with a planar radiating patch, a dielectric substrate, a ground plane, and an inset microstrip feed line designed for standard $50\,\Omega$ characteristic impedance matching.

<p align="center">
  <img src="https://raw.githubusercontent.com/RAKESHBALAJI2182/patch-antenna-2.4ghz/main/antenna_geometry.png" alt="Microstrip Patch Antenna Geometry" width="650"/>
</p>

- **Configuration:** Inset / Line-Fed Rectangular Microstrip Patch Antenna
- **Target Band:** $2.4\text{ GHz}$ ISM (Industrial, Scientific, and Medical)
- **Excitation:** Waveguide Port aligned with the feedline microstrip cross-section

---

## 📊 Simulation & Results

The antenna was analyzed using the Transient Solver in CST Studio Suite across multiple mesh refinement passes (`Mesh Pass = 1` and `Mesh Pass = 2`) to ensure spatial convergence and numerical stability.

### 1. Return Loss ($S_{11}$)
- **Resonant Frequency:** $2.40\text{ GHz}$
- **Return Loss ($S_{11}$):** $\mathbf{-11.3\text{ dB}}$ at $2.40\text{ GHz}$

<p align="center">
  <img src="https://raw.githubusercontent.com/RAKESHBALAJI2182/patch-antenna-2.4ghz/main/s11_plot.png" alt="S11 Return Loss" width="700"/>
</p>

### 2. Voltage Standing Wave Ratio (VSWR)
- **VSWR at Resonance:** $\approx \mathbf{1.75}$ at $2.40\text{ GHz}$ (satisfies standard $\le 2:1$ operational bandwidth limits)

<p align="center">
  <img src="https://raw.githubusercontent.com/RAKESHBALAJI2182/patch-antenna-2.4ghz/main/vswr_plot.png" alt="VSWR vs Frequency" width="700"/>
</p>

---

## 📁 Repository Contents

| File | Description |
| :--- | :--- |
| `microstrip_patch_antenna.cst` | CST Studio Suite 3D simulation model file (`EZPAB.cst`) |
| `antenna_geometry.png` | 3D perspective CAD render showing patch, inset notch, and waveguide port |
| `s11_plot.png` | Converged S11 reflection coefficient vs. frequency |
| `vswr_plot.png` | VSWR characteristic curve across 2–3 GHz |
| `README.md` | Comprehensive design and simulation report |

---
**Tool:** CST Studio Suite  
**Author:** Bollam Rakesh Balaji (NIT Mizoram)