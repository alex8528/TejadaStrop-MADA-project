# Code

This folder contains all scripts used in the analysis pipeline.

## Processing
- `processing/01_load_clean.qmd`  
- `processing/02_create_analytic_dataset.qmd`  

## Exploratory Analysis
- `eda/03_exploratory_analysis.qmd`  

## Statistical Analysis
- `analysis/04_statistical_analysis.qmd`  
- `analysis/05_model_validation.qmd`  

## Notes
Scripts are numbered to indicate the order in which they should be run.

The raw PRAMS Excel file may be too large to process in some environments. A processed analytic dataset is provided in data/processed-data so the remaining workflow can be reproduced.