---
title: 'Introduction to Radiative Transfers'
permalink: /theory/Radiative_Transfer
tags:
  - Radiative Transfer
  - RT
  - Monte Carlo
  - MCRT
  - Emission
  - Reprocessing
  - SEDONA
---
The information we can extract from observations of astrophysical systems relies heavily on our understanding of electromagnetic radiation. To interpret these observations, we must model the production and transport of radiation. Therefore, radiative transfer is a fundamental process in astrophysics that describes how electromagnetic radiation propagates through and interacts with matter


Radiative Transfer
====
Radiation processes are complex and computationally demanding due to their high dimensionality. The radiation field generally depends on three spatial dimensions and three momentum directions (frequency and two angles), resulting in a six-dimensional time-dependent solution that requires computational techniques to solve (Roth&Kasen, 2015), not to mention the case when polarisation also needs to be studied. To reduce dimensionality and complexity, various numerical methods have been employed, such as neglecting angular dependencies (e.g. M1 closure, Pomraning, 1969), frequency (e.g. grey opacity Eddington, 1926), temporal dependence (steady-state), or assuming spatial symmetry (e.g. spherical). Monte Carlo Radiative Transfer (MCRT) methods are among the most versatile approaches, as they enable the treatment of the problem in its full dimensionality and are well-suited for parallelization on computing clusters. The code I use for my research is a MCRT code called Sedona (Kasen et al., 2006). In the following sections, I present the radiative transfer equation, which dictates how radiation is transported, and then the Monte Carlo approach to solving it.


