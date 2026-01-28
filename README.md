# Patch Antenna Design and Simulation in HFSS

This repository contains the simulation results of a microstrip patch antenna designed and analyzed using **Ansys HFSS**.  
The project focuses on antenna geometry design, impedance matching, and radiation characteristics at the target frequency.

---

## Antenna Geometry

- PCB size: **100 × 100 mm**
- Corner cutouts: **10 × 10 mm** (each corner)
- Central circular cutout: **radius = 18 mm**
- Patch antenna dimensions: **6.36 × 9.04 mm**
- Feed port dimensions: **1.6 × 2.9 mm**

The geometry was designed to operate in the **Ku-band** with emphasis on compact patch elements and proper impedance matching.

---

## Materials and Boundary Conditions

- **Substrate:** FR4_epoxy  
- **Feed type:** Lumped Port  
- **Ground plane:** Perfect Electric Conductor (Perfect E)  
- **Surrounding medium:** Air (vacuum region)

---

## Operating Frequency

The operating (resonant) frequency of the antenna is identified from the **S-parameter (S11)** response:

- **Resonant frequency:** **12.62 GHz**
- **Return loss:** below −40 dB at resonance, indicating good impedance matching

---

## Input Impedance Analysis

From the **Terminal Z-parameter** plot, the input impedance at the resonant frequency can be observed:

- **Input impedance at 12.62 GHz:** **≈ 49.72 Ω**

This value is close to the standard **50 Ω**, confirming proper impedance matching between the feed and the antenna at the operating frequency.

---

## Radiation Characteristics

- **Radiation pattern type:** Directional
- **Reported quantity:** GainTotal (3D radiation pattern)
- The radiation pattern demonstrates a dominant main lobe at the operating frequency.

---

## Electric Field Distribution

The electric field distribution shows energy concentration near the feed region and patch elements, confirming correct excitation and power transfer from the feed to the radiating structure.

---

## Notes

This project demonstrates practical experience in:
- Antenna geometry design
- Electromagnetic simulation using HFSS
- S-parameter and impedance analysis
- Radiation pattern evaluation

The model is intended for simulation and academic demonstration purposes.
