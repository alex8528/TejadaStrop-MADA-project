## Project Workflow

This project follows a reproducible analysis pipeline:

Raw PRAMS data  
↓  
Data cleaning and processing  
↓  
Analytic dataset creation  
↓  
Exploratory analysis  
↓  
Regression modeling and model validation  
↓  
Tables and figures  
↓  
Manuscript and portfolio page

### Reproduction steps

To reproduce the project, run the files in this order:

1. `code/processing-code/01_load_clean.qmd`
2. `code/processing-code/02_create_analytic_dataset.qmd`
3. `code/eda-code/03_exploratory_analysis.qmd`
4. `code/analysis-code/04_model_validation.qmd`
5. `quarto render products/manuscript/Manuscript.qmd`