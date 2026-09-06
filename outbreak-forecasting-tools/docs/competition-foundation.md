# 2026 Influenza Forecasting Competition: Methodological Foundation

## Background

This module builds on forecasting work developed for the 2026 Modeling the Invisible Forecasting Competition, which focused on short-term prediction of influenza-associated hospitalization dynamics.

The original competition implementation is preserved in the separate repository:

[`modeling-the-invisible-2026`](https://github.com/maruf-lawal/modeling-the-invisible-2026)

That repository contains the original competition notebook and is retained as the historical implementation record.

## Forecasting Approach

The competition framework combined multiple forecasting approaches, including:

- a mechanistic SIR-H epidemic model;
- ETS time-series forecasting;
- ARIMA forecasting;
- trend-based forecasting;
- direct forecasting approaches; and
- adaptive ensemble weighting.

The purpose of the ensemble design was to combine complementary forecasting approaches rather than rely on a single model class.

## Role in the Current Research Framework

The present forecasting module extends the competition work in several directions.

Planned methodological development includes:

- systematic retrospective and rolling-origin evaluation;
- more explicit comparison of individual model components;
- improved documentation of model assumptions and preprocessing;
- uncertainty-aware and probabilistic forecasting;
- alternative ensemble-weighting strategies;
- standardized evaluation workflows; and
- reproducible forecasting pipelines that can be updated as new influenza surveillance data become available.

The current framework therefore treats the competition implementation as a methodological starting point rather than as a completed forecasting platform.

## Reproducibility

Where appropriate, forecasting methods developed from the competition work will be reorganized into documented scripts, notebooks, and evaluation workflows within this module.

The original competition repository will remain separate so that the historical implementation is preserved and distinguishable from later research development.
