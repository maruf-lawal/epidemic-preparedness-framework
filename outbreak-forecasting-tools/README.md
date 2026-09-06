# Hybrid Influenza Forecasting and Early Warning

## Overview

This module develops and evaluates **short-term influenza forecasting methods** that combine mechanistic epidemic models with statistical and data-driven approaches.

It is one of three interconnected components of the broader [Epidemic Preparedness Framework](../README.md), whose current research focus is seasonal and emerging influenza threats in the United States.

The principal goals of this module are to:

- develop reproducible short-term influenza forecasting workflows;
- compare mechanistic, statistical, and hybrid forecasting approaches;
- investigate adaptive ensemble methods;
- quantify and evaluate forecast uncertainty;
- assess performance using sequential and retrospective validation; and
- develop methods that can be extended as new influenza surveillance data become available.

## Existing Foundation: 2026 Influenza Forecasting Competition

Development of this module builds on work completed for the **2026 Modeling the Invisible Forecasting Competition**, in which our team developed a forecasting framework for predicting influenza-associated hospitalization dynamics.

The competition approach combined:

- a mechanistic **SIR-H** epidemic model;
- **ETS** time-series forecasting;
- **ARIMA** forecasting;
- trend-based forecasting;
- direct forecasting approaches; and
- adaptive ensemble weighting.

The original competition implementation is preserved separately in the [`modeling-the-invisible-2026`](https://github.com/maruf-lawal/modeling-the-invisible-2026) repository.

That repository is maintained as the record of the original competition implementation. This module is intended to extend the underlying forecasting work into a broader research framework for systematic validation, uncertainty assessment, and continued methodological development.

## Research Objectives

### 1. Mechanistic Forecasting

Develop and evaluate compartmental influenza models that represent relevant transmission and hospitalization dynamics and can be updated as surveillance observations become available.

Initial development builds on the SIR-H structure used in the 2026 forecasting competition.

### 2. Statistical Forecasting

Evaluate statistical and time-series methods for short-term prediction of influenza-associated outcomes, including approaches such as ETS, ARIMA, trend-based models, and other appropriate forecasting methods.

### 3. Hybrid and Ensemble Forecasting

Investigate combinations of mechanistic and statistical forecasts using adaptive ensemble methods.

A central research question is whether dynamically weighting complementary forecasting approaches can improve predictive accuracy, stability, or robustness across different phases of an influenza season.

### 4. Forecast Uncertainty

Extend point forecasting approaches to incorporate and evaluate predictive uncertainty.

Development will include appropriate interval or probabilistic forecasting methods as the framework matures.

### 5. Sequential and Retrospective Validation

Forecasts will be evaluated using rolling-origin, sequential, or retrospective designs that approximate the information available at the time a forecast would have been generated.

Evaluation will consider appropriate measures of:

- predictive accuracy;
- forecast calibration;
- uncertainty;
- stability across forecasting rounds; and
- comparative performance of individual and ensemble models.

## Data

Development will use publicly available influenza surveillance and hospitalization data where appropriate.

Data sources, preprocessing procedures, transformations, and any applicable use restrictions will be documented as datasets are incorporated into the module.

Large or externally maintained datasets will generally not be duplicated in this repository when they can instead be obtained directly from their authoritative source.

## Planned Module Structure

As implementation progresses, this module is expected to contain components such as:

```text
outbreak-forecasting-tools/
│
├── README.md
├── LICENSE
├── models/
│   ├── mechanistic/
│   └── statistical/
├── code/
├── data/
├── evaluation/
├── figures/
├── results/
└── docs/
```

Directories will be added as substantive materials become available rather than as empty placeholders.

## Development Roadmap

Current development priorities are:

1. document and reproduce the principal forecasting approaches used in the 2026 influenza forecasting competition;
2. establish a standardized workflow for comparing individual forecasting models;
3. implement retrospective and rolling forecast evaluation;
4. extend the ensemble framework to incorporate uncertainty;
5. evaluate alternative ensemble weighting strategies;
6. document data sources and preprocessing procedures; and
7. release reproducible examples, figures, and evaluation results as the research progresses.

## Relationship to the Broader Framework

This forecasting module is being developed alongside:

- **behaviorally informed influenza vaccination modeling**, which investigates how vaccination behavior and changing risk perception influence epidemic dynamics; and
- **risk-aware intervention optimization**, which evaluates time-dependent intervention strategies under epidemiological, resource, and uncertainty constraints.

The longer-term research objective is to investigate how forecasting information can interact with behavioral modeling and intervention optimization within a modular influenza preparedness framework.

## Reproducibility

Code and documentation will be organized to support transparent and reproducible analysis.

As individual forecasting components are implemented, the repository will document:

- model assumptions;
- parameter definitions;
- software requirements;
- data sources and preprocessing;
- forecast-generation procedures;
- evaluation methods; and
- instructions for reproducing principal results.

## Status

**Active development.**

The original 2026 influenza competition implementation is already available in the separate [`modeling-the-invisible-2026`](https://github.com/maruf-lawal/modeling-the-invisible-2026) repository.

This module is being developed as an extension of that work rather than as a replacement for the original competition repository.

## Author

**Maruf A. Lawal**  
Department of Mathematics  
University of Tennessee, Knoxville

Research interests: mathematical epidemiology, outbreak forecasting, mathematical biology, data science, machine learning, and optimal control.

## License

This module is distributed under the MIT License. See the [LICENSE](LICENSE) file for details.
