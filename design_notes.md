# Antenna Design Notes

This document describes the initial design approach used to determine the dimensions of the microstrip patch antenna prior to full-wave simulation.

---

## Patch Dimension Estimation

The initial width (W) of the rectangular patch antenna was estimated using standard analytical expressions commonly used in microstrip antenna design:

W = c / (2 f₀ √((εᵣ + 1)/2))

where:
- c is the speed of light,
- f₀ is the target operating frequency,
- εᵣ is the relative permittivity of the substrate.

---

## Effective Dielectric Constant

Due to fringing fields at the patch edges, an effective dielectric constant ε_eff was used:

ε_eff = (εᵣ + 1)/2 + (εᵣ − 1)/2 · [1 / √(1 + 12h/W)]

where h is the substrate thickness.

---

## Effective Patch Length

The effective length of the patch was calculated as:

L = c / (2 f₀ √(ε_eff)) − ΔL

where ΔL represents the length extension caused by fringing effects.

These analytical expressions provide initial design values only. Final antenna dimensions were refined using full-wave electromagnetic simulation in Ansys HFSS.

---

## Element Spacing Considerations

For multi-element configurations, the spacing between adjacent patch antennas is typically chosen close to λ/2 at the operating frequency. This spacing provides a balance between array compactness and reduced mutual coupling.

---

## Design Approach Summary

1. Initial antenna dimensions were calculated using analytical formulas and online microstrip antenna calculators.
2. The geometry was implemented in Ansys HFSS.
3. Full-wave simulation was used to evaluate S-parameters, input impedance, radiation pattern, and field distribution.
4. Final performance was verified at the resonant frequency of 12.62 GHz.
