# Early-Life Immune Activation and Risk of House Dust Allergy - Observational Analysis Using the PRINCE Cohort Study

## Introduction

Clinical observations in pediatrics suggest that early-life infections or immune activation may increase the risk of later allergic sensitization, including house dust mite allergy. Understanding whether such associations are supported by empirical longitudinal data is crucial for refining early prevention strategies and for improving early-life risk stratification.

The present project uses data from the PRINCE Study (Prenatal Identification of Children’s Health), a prospective observational cohort conducted at the Universitäres Perinatalzentrum, Universitätsklinikum Hamburg-Eppendorf (UKE). The PRINCE Study follows families from the first trimester of pregnancy through childhood, collecting comprehensive prenatal, perinatal, and postnatal data including clinical parameters, questionnaires, and biological samples.

This repository contains the analytical framework to investigate whether early immune activation events are associated with an elevated risk of developing house dust allergy in childhood.

## Objective

The aim of this analysis is to evaluate whether infections or immune activation occurring in early life (prenatal or early postnatal) predict later development of house dust allergy. Specifically, we examine:
- the association between early-life immune-related events and subsequent allergic outcomes
- potential confounding factors such as sex, parental atopy, environmental exposures, socioeconomic indicators, and early-life nutrition
- whether timing of immune activation (prenatal vs. postnatal) modifies allergy risk

The analysis is exploratory but aims to generate clinically meaningful hypotheses for further mechanistic studies.

## Methodological Overview

The project uses an observational design based on the PRINCE cohort’s longitudinal data. The analytical workflow includes:
- preprocessing and harmonization of repeated measures and clinical variables
- construction of exposure variables describing early-life immune activation
- definition of outcome variables based on clinically verified house dust allergy markers
- confounder selection guided by directed acyclic graphs (DAGs) and domain expertise
- regression-based association models with sensitivity analyses
- robustness checks including alternative exposure definitions and missing-data handling strategies

All analyses are performed in R, following reproducible research principles.

## Project Structure

- **`data/`**: Contains the dataset used in the analysis.
- **`scr/`**: R scripts for data exploration, preprocessing, modeling, and assumption testing.
- **`graphs/`**: Figures and visualizations produced during the analytical workflow.

## Scripts

- **Analysis.ipynb**: This script conducts the core statistical analyses.

## Acknowledgements

Statistical analysis and methodological development were conducted by
**Dr. Steven Ngandeu Schepanski.** The PRINCE Study team at the Universitätsklinikum Hamburg-Eppendorf is gratefully acknowledged for providing access to the cohort data.

## Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/sschepanski/HouseDust_PRINCE.git
   ```
2. **Set up your R environment:**
   Ensure that R is installed and configured. All required packages are integrated directly in the respective R scripts. When running a script, any missing packages will be prompted for installation.
3. **Run the provided R scripts:**
   Execute the R scripts found in the scr/ directory for data preprocessing, modeling, and assumption testing. Set your working directory to the root of the project to ensure smooth execution of the scripts.

## Contributions

This repository is part of an ongoing research collaboration investigating early-life determinants of childhood health, with a focus on immune development and allergic disease.

## License

This project is licensed under the MIT License.