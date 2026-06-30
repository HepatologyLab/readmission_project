# Tacrolimus Variability and Creatinine Predict Readmission After Liver Transplantation

This repository contains the analysis code supporting the manuscript:

> Korenblat K. Tacrolimus Variability and Creatinine Predict Readmission After Liver Transplantation. [Journal, year, in submission/press]

## Overview

This study used time-varying Cox proportional hazards regression and gradient-boosted machine learning (XGBoost) to:

1. Identify the readmission window most predictive of 1-year mortality after liver transplantation, using a time-varying covariate approach to correct for immortal time bias.
2. Develop and cross-validate models predicting 90-day unplanned readmission using laboratory and clinical data available through postoperative day 7, compared to models using complete hospitalization data.
3. Identify and characterize the interaction between tacrolimus coefficient of variation and peak serum creatinine as a predictor of readmission risk.

## What This Repository Contains

This repository contains the **analysis pipeline only**: feature engineering, model development, cross-validation, calibration assessment, and statistical analysis (R/Quarto).

This repository does **not** contain:
- Patient-level data of any kind
- Data extraction or query scripts used to pull records from the electronic health record
- Data cleaning or de-identification scripts

Data extraction and cleaning were performed separately against the institution's electronic health record system and involved protected health information; those scripts are not shared, consistent with institutional data governance and patient privacy requirements. See the manuscript's Data Availability Statement for details on the dataset and the process for requesting restricted access.

## Repository Structure

| File/Folder | Description |
|---|---|
| `[update with actual filenames]` | Feature engineering: construction of tacrolimus coefficient of variation, peak creatinine, and other laboratory trajectory features from cleaned input data |
| `[update with actual filenames]` | Time-varying Cox regression models and immortal time bias correction |
| `[update with actual filenames]` | XGBoost model training, 5-fold cross-validation, and hyperparameter handling |
| `[update with actual filenames]` | Calibration analysis (Brier score, calibration plots) |
| `[update with actual filenames]` | Figure and table generation |

*(Update this table with your actual file names once finalized.)*

## Software and Dependencies

Analysis was performed in R version [fill in], using the following key packages:

- `data.table`
- `xgboost`
- `survival`
- `ggplot2`
- `flextable`
- `pROC`
- `here`

A full session info / package version list is available in `[add file name if you choose to include one, e.g., sessionInfo.txt]`.

## Reproducibility Note

Because the input dataset cannot be shared (see above), this code cannot be run end-to-end without access to a structurally equivalent dataset. The code is provided to support transparency of methods and to allow evaluation of the analytical approach, consistent with PLOS ONE's reproducibility and code-sharing requirements. A researcher with access to a comparable dataset (consistent variable structure, as described in the manuscript Methods) could adapt this pipeline directly.

## AI Assistance Disclosure

Portions of this code were developed with assistance from Claude (Anthropic), a large language model used as a coding assistant. All code was reviewed, tested, and validated by the author. Study design, data interpretation, and all scientific conclusions are solely the work of the author. See the manuscript Methods section for full disclosure.

## Citation

If you use this code, please cite the manuscript above. A full citation will be added upon publication.

## Contact

Kevin Korenblat, MD
Washington University School of Medicine

