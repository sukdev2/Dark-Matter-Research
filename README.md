# Dark Matter Propagation in the Sun using Non-Relativistic Effective Field Theory (NR-EFT)

![Python](https://img.shields.io/badge/Python-3.11%2B-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Field](https://img.shields.io/badge/Field-Astroparticle%20Physics-green.svg)
![Status](https://img.shields.io/badge/Status-Ongoing-yellow.svg)

Numerical study of heavy dark matter capture, propagation, thermalization, and related phenomenology inside the Sun within the framework of **Non-Relativistic Effective Field Theory (NR-EFT)**.

---

## Overview

This repository contains the **Python/Jupyter Notebook implementations, numerical calculations, intermediate results, and analysis developed during my M.Sc. research in Dark Matter Physics**.

The project investigates the capture and subsequent evolution of heavy dark matter particles inside the Sun. The main focus is on dark matter–nucleus interactions described within the **Non-Relativistic Effective Field Theory (NR-EFT)** framework and on understanding how the properties of these interactions affect dark matter propagation and thermalization in the solar interior.

The study considers heavy dark matter in the **TeV–PeV mass regime**, where the fractional energy loss per scattering becomes increasingly suppressed. This can lead to inefficient thermalization and the persistence of extended, non-thermal orbits inside the Sun.

The numerical calculations use realistic solar-model data, operator-dependent nuclear response functions, and numerical integration of the relevant scattering and capture expressions.

The repository is intended to provide a structured record of the computational work associated with the M.Sc. thesis and to support reproducibility, validation, further analysis, and future development.

---

## Research Project

### Propagation of TeV–PeV Scale Dark Matter in the Sun within the Framework of Non-Relativistic Effective Field Theory (NR-EFT)

**Research Area:** Astroparticle Physics · Dark Matter Phenomenology · Non-Relativistic Effective Field Theory · Computational Physics

The central objective of the project is to study the evolution of heavy dark matter after gravitational capture by the Sun, with particular emphasis on the scattering dynamics, orbital evolution, and thermalization of dark matter in the solar interior.

The theoretical framework focuses primarily on the NR-EFT operators

$\hat{O}_4$ \, \hat{O}_8$ \, \hat{O}_{15}$

which represent different types of dark matter–nucleon interactions involving spin, velocity, and momentum dependence.

---

## Scientific Motivation

Dark matter particles passing through the Sun can lose kinetic energy through scattering with solar nuclei. If sufficient energy is lost, the particles become gravitationally bound to the Sun.

For conventional WIMP masses, repeated scattering can eventually bring the captured dark matter population toward thermal equilibrium with the solar medium. However, for sufficiently heavy dark matter, the fractional energy loss in an individual scattering event becomes small.

Consequently :

- capture can occur without rapid thermalization,
- dark matter can remain on extended non-thermal orbits,
- the spatial distribution of dark matter can differ substantially from the standard thermal-equilibrium distribution,
- the annihilation rate can be significantly affected,
- and the resulting neutrino signal can differ from conventional solar dark-matter scenarios.

The heavy-dark-matter regime is therefore particularly interesting for studying the limitations of the standard assumption of rapid thermalization. The thesis framework specifically investigates this non-thermal evolution. :contentReference[oaicite:2]{index=2}

---

## Scientific Objectives

The overall objectives of the M.Sc. thesis are:

1. **Calculate dark matter capture in the Sun.**
2. Study dark matter–nucleus scattering within the NR-EFT framework.
3. Incorporate operator-dependent nuclear response functions.
4. Compare the effects of different NR-EFT operators.
5. Study the propagation of gravitationally captured dark matter inside the Sun.
6. Investigate the orbital evolution of captured dark matter.
7. Study the thermalization process through repeated scattering.
8. Determine the resulting non-thermal dark matter distribution.
9. Estimate the dark matter annihilation rate in the solar interior.
10. Investigate the corresponding neutrino flux at Earth.
11. Compare the numerical results with theoretical calculations and results available in the literature.

---

## NR-EFT Operators

The present study focuses primarily on:

### $\hat{O}_4$

A spin-dependent NR-EFT interaction.

### $\hat{O}_8$

A velocity-dependent interaction involving the dark matter transverse velocity.

### $\hat{O}_{15}$

A momentum- and velocity-dependent interaction with corresponding nuclear response contributions.

The different operators lead to different scattering behaviour because they couple to different nuclear response functions. Consequently, the capture and subsequent propagation of dark matter can depend strongly on the underlying operator.

---

## Solar Models

The numerical calculations use realistic solar-model profiles.

The current implementation includes:

- **BP2000**
- **AGSS09**

The solar profiles provide quantities such as:

- radial coordinate,
- solar density,
- hydrogen abundance,
- iron abundance,
- phosphorus abundance,
- enclosed solar mass,
- and escape velocity.

These quantities are incorporated into the numerical capture calculation.

---

## Target Nuclei

The current capture calculation considers three representative solar target nuclei:

- Hydrogen (H)
- Iron (Fe)
- Phosphorus (P)

The capture rate is calculated separately for each element and then combined to obtain the total capture rate.

---

## Capture Rate Calculation

The current repository contains a structured implementation of the solar dark-matter capture calculation.

The calculation includes:

- Natural-unit conversions
- Solar-model loading
- Solar density profiles
- Elemental abundances
- Solar mass profile
- Solar escape velocity
- Dark-matter velocity distribution
- WIMP–nucleus reduced mass
- Kinematic energy limits
- Nuclear response functions
- WIMP response functions
- Differential scattering cross sections
- Radial integration
- Velocity integration
- Recoil-energy integration
- Element-by-element capture rates
- Total capture rate

The capture calculation is performed for the NR-EFT operators $\hat{O}_4$, $\hat{O}_8$, and $\hat{O}_{15}$ and for both **isoscalar** and **isovector** couplings.

The current calculation produces structured numerical results for:

H
Fe
P
Total

## Key Research References

The theoretical framework and numerical methodology of this project are primarily based on the following studies.

### 1. NR-EFT Dark Matter Capture and Nuclear Response Functions

**R. Catena and B. Schwabe**,  
*"Form factors for dark matter capture by the Sun in effective theories,"*  
Journal of Cosmology and Astroparticle Physics **04 (2015) 042**.

[arXiv:1501.03729](https://arxiv.org/abs/1501.03729)  
DOI: [10.1088/1475-7516/2015/04/042](https://doi.org/10.1088/1475-7516/2015/04/042)

This work provides the nuclear response functions and formalism used to study dark matter capture in the Sun within the non-relativistic effective theory framework. It considers isoscalar and isovector dark matter–nucleon interactions and calculates nuclear response functions for the elements relevant to the solar capture process.

The present capture-rate calculation follows this theoretical framework, with the implementation adapted to the solar-model data and numerical setup used in this project.
