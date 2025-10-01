# Longitudinal LME Analysis of the DESCRIBE Dataset

This repository contains R scripts and outputs for performing **longitudinal analysis of neuropsychiatric symptoms** using **Linear Mixed-Effects (LME) models** on the **DESCRIBE dataset**.

## Overview

The goal of this project is to model disease progression across different variants of **Frontotemporal Dementia (FTD)** and **Primary Progressive Aphasia (PPA)** by analyzing longitudinal symptom trajectories.

## Data

* **Dataset**: DESCRIBE
* **Groups**:

  * bvFTD (behavioral variant FTD)
  * nsPPA (unspecified PPA)
  * nfPPA (non-fluent PPA)
  * lvPPA (logopenic PPA)
  * svPPA (semantic PPA)
* **Phenotypes (from PCA clustering)**:

  * Active behavioral symptoms
  * Passive behavioral symptoms
  * Affective symptoms
  * Psychotic symptoms

## Methods

* Data preprocessing: cleaning, variable creation (e.g., **EYO – Estimated Years to Onset**).
* Statistical modeling: Linear Mixed-Effects models using `lme4`.
* Fixed effects tested: **EYO, diagnosis group, gender, age, MMSE, education**.
* Random effects: subject (Code), family, acquisition site.
* Model comparison with **AIC, BIC, R² (marginal/conditional), ICC, likelihood ratio tests**.
* Visualization of symptom trajectories and model diagnostics.

## Outputs

* Estimates of group differences in symptom progression.
* Significance testing with Wald chi-square and Monte Carlo simulations.
* Graphical validation: residual diagnostics, normality, homogeneity, collinearity.
* Comparative figures of longitudinal trajectories across diagnostic groups.

## Requirements

* R (≥ 4.0)
* Packages: `lme4`, `car`, `performance`, `jtools`, `ggplot2`, `dplyr`, `tidyverse`, `kableExtra`, `readxl`, `huxtable`, `lattice`.

## Citation

If you use this code or analysis, please cite:
*CITE OF THE PAPER*
