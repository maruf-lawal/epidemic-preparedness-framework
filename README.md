# Epidemic Preparedness Framework

A modular computational research framework for integrating **behaviorally informed epidemic modeling, intervention optimization, and outbreak forecasting**, with current development focused on applications to **seasonal and emerging influenza threats in the United States**.

## Overview

Effective infectious-disease preparedness requires more than estimating transmission dynamics. Public-health decisions may also depend on how individuals respond to changing risk, how limited interventions should be allocated over time, and how reliably near-term disease burden can be forecast.

This repository provides a modular framework for developing and evaluating quantitative methods across three interconnected areas:

1. **Behaviorally Informed Vaccination Modeling**  
   Mathematical models that incorporate dynamic vaccination behavior, vaccine hesitancy, perceived risk, and responsiveness to epidemiological information.

2. **Multi-Intervention Optimization**  
   Optimal-control and decision-analysis methods for evaluating combinations of vaccination, treatment, testing, public-health outreach, and other interventions under epidemiological and resource constraints.

3. **Hybrid Outbreak Forecasting**  
   Forecasting approaches that combine mechanistic epidemic models with statistical and data-driven methods, with emphasis on predictive validation and uncertainty.

The framework is designed to be modular and reproducible so that individual components can be developed, evaluated, and integrated as the research progresses.

## Current Research Focus: Influenza Preparedness

Current development focuses on adapting and integrating these methods for **influenza preparedness and public-health decision support**.

The influenza-focused research program has three principal components:

### 1. Behaviorally Informed Influenza Vaccination Modeling

This component investigates how vaccination behavior and changes in perceived risk can influence influenza transmission and intervention outcomes.

Planned development includes:

- dynamic vaccination uptake and hesitancy;
- behavioral responses to epidemiological information;
- delayed changes in risk perception and vaccine acceptance;
- calibration using relevant U.S. influenza and vaccination data;
- sensitivity and uncertainty analysis; and
- evaluation of vaccination and public-health outreach strategies.

### 2. Risk-Aware Influenza Intervention Optimization

This component develops mathematical methods for comparing and optimizing combinations of influenza interventions over time.

Potential intervention variables include:

- vaccination;
- antiviral treatment;
- diagnostic testing;
- public-health outreach; and
- appropriate non-pharmaceutical interventions.

The framework will incorporate epidemiological and resource constraints and will progressively evaluate robustness to uncertainty in transmission, intervention effectiveness, uptake, and resource availability.

### 3. Hybrid Influenza Forecasting and Early Warning

This component develops short-term influenza forecasting methods by combining mechanistic epidemic models with statistical and data-driven approaches.

The work builds on experience from the **2026 Modeling the Invisible Forecasting Competition**, in which our team developed an adaptive ensemble for forecasting influenza-associated hospitalizations using mechanistic SIR-H modeling together with ETS, ARIMA, trend-based, and direct forecasting approaches.

The original competition implementation is preserved separately in the [`modeling-the-invisible-2026`](https://github.com/maruf-lawal/modeling-the-invisible-2026) repository.

Current and future development will investigate:

- adaptive ensemble forecasting;
- sequential model updating;
- forecast uncertainty;
- rolling and retrospective validation;
- comparison of mechanistic and statistical approaches; and
- reproducible forecasting workflows.

## Repository Structure

The framework is organized around three methodological modules:

```text
epidemic-preparedness-framework/
│
├── vaccine-hesitancy-optimization/
│   └── Behavioral epidemic modeling and vaccination dynamics
│
├── multi-intervention-optimal-control/
│   └── Dynamic intervention optimization under constraints
│
├── outbreak-forecasting-tools/
│   └── Mechanistic, statistical, and hybrid forecasting methods
│
├── LICENSE
└── README.md
