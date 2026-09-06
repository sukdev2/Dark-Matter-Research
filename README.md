# Dark Matter Propagation in the Sun using Non-Relativistic Effective Field Theory (NR-EFT)

![Python](https://img.shields.io/badge/Python-3.11%2B-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Field](https://img.shields.io/badge/Field-Astroparticle%20Physics-green.svg)
![Status](https://img.shields.io/badge/Status-Ongoing-yellow.svg)

Numerical study of heavy dark matter capture, propagation, and thermalization inside the Sun within the framework of **Non-Relativistic Effective Field Theory (NR-EFT)**.

---

## Overview

This repository contains the **Python/Jupyter Notebook calculations, numerical results, and analysis** developed during my M.Sc. research in Dark Matter Physics.

The project studies the capture and subsequent evolution of heavy dark matter inside the Sun, with emphasis on **NR-EFT dark matter–nucleus interactions**, orbital evolution, and thermalization.

The study focuses on the **TeV–PeV dark matter mass regime**, where energy loss per scattering can be small, leading to inefficient thermalization and extended non-thermal orbits.

---

## Research Objectives

- Calculate dark matter capture in the Sun.
- Study dark matter–nucleus scattering using NR-EFT.
- Implement operator-dependent nuclear response functions.
- Study propagation and orbital evolution after capture.
- Investigate thermalization through repeated scattering.
- Determine the resulting non-thermal dark matter distribution.
- Study dark matter annihilation inside the Sun.
- Investigate the resulting neutrino flux at Earth.
- Compare numerical results with the literature.

---

## NR-EFT Operators

The present study focuses on:

- $\hat{O}_4$ — spin-dependent interaction
- $\hat{O}_8$ — velocity-dependent interaction
- $\hat{O}_{15}$ — momentum- and velocity-dependent interaction

Different operators produce different scattering rates through their corresponding nuclear response functions.

---

## Solar Models

The current implementation uses:

- **BP2000**
- **AGSS09**

The solar-model data provide the radial profiles required for the capture calculation, including density, elemental abundances, enclosed mass, and escape velocity.

---

## Target Nuclei

The current capture calculation includes:

- Hydrogen (H)
- Iron (Fe)
- Phosphorus (P)

Individual capture rates are calculated for each element and combined to obtain the **total capture rate**.

---

## Capture Rate Calculation

The current **capture-rate calculation is the completed and structured part of the repository**.

It includes:

- Solar-model data
- Dark-matter velocity distribution
- Reduced masses and kinematic limits
- Nuclear and WIMP response functions
- Differential scattering cross sections
- Radial integration
- Velocity integration
- Recoil-energy integration
- Element-by-element capture rates
- Total capture rates

The calculation is performed for $\hat{O}_4$, $\hat{O}_8$, and $\hat{O}_{15}$ with both **isoscalar** and **isovector** couplings.

Results are stored separately for:

H
Fe
P
Total

## Key Research References The theoretical framework and numerical methodology of this project are primarily based on the following studies. 

### 1. NR-EFT Dark Matter Capture and Nuclear Response Functions 

**R. Catena and B. Schwabe**, 

*"Form factors for dark matter capture by the Sun in effective theories,"* Journal of Cosmology and Astroparticle Physics 

**04 (2015) 042**. [arXiv:1501.03729](https://arxiv.org/abs/1501.03729) DOI: [10.1088/1475-7516/2015/04/042](https://doi.org/10.1088/1475-7516/2015/04/042) 

This work provides the nuclear response functions and formalism used to study dark matter capture in the Sun within the non-relativistic effective theory framework. It considers isoscalar and isovector dark matter–nucleon interactions and calculates nuclear response functions for the elements relevant to the solar capture process. The present capture-rate calculation follows this theoretical framework, with the implementation adapted to the solar-model data and numerical setup used in this project.
