# Prenatal Mental Health Screening and Postpartum Depressive Symptoms

## Project Overview

This project examines whether prenatal mental health screening is associated with postpartum depressive symptoms using data from the Pregnancy Risk Assessment Monitoring System (PRAMS) Phase 8. 

The analysis evaluates whether individuals who report being asked about depression or anxiety during prenatal care are less likely to report postpartum depressive symptoms.


## Project Workflow

The project follows a reproducible analysis pipeline:

raw data → data processing → analytic dataset → exploratory analysis → modeling → manuscript

All datasets, tables, and figures are generated using code.

## Repository Structure

Key files and folders include:

- `code/processing/01_load_clean.qmd`  
  Loads and cleans the raw PRAMS dataset.

- `code/processing/02_create_analytic_dataset.qmd`  
  Creates the final analytic dataset.

- `code/eda/03_exploratory_analysis.qmd`  
  Generates descriptive tables and figures.

- `code/analysis/04_statistical_analysis.qmd`  
  Runs logistic regression models.

- `code/analysis/05_model_validation.qmd`  
  Performs 5-fold cross-validation and compares logistic regression and random forest models.

- `products/manuscript/Manuscript.qmd`  
  Contains the final manuscript.

## Data

- Raw data: `data/raw-data/`  
- Processed data: `data/processed-data/`  
- Results:  
  - Tables: `results/tables/`  
  - Figures: `results/figures/`  

Processed datasets are saved as `.rds` files to preserve variable types.

## Reproducibility

To reproduce the analysis, run the following scripts in order:

1. `code/processing/01_load_clean.qmd`
2. `code/processing/02_create_analytic_dataset.qmd`
3. `code/eda/03_exploratory_analysis.qmd`
4. `code/analysis/04_statistical_analysis.qmd`
5. `code/analysis/05_model_validation.qmd`


The manuscript loads all tables, figures, and model outputs generated during analysis.

## Main Research Question

Are individuals who report being asked about depression or anxiety during prenatal care less likely to report postpartum depressive symptoms?

## Software

This project was developed using:

- R  
- Quarto  

Key R packages:

- tidyverse  
- tidymodels  
- broom  
- knitr  
- here  
- kableExtra  
- survey  


## Author

Alexandra Tejada-Strop
