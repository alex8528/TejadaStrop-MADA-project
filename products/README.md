## Reproducibility

Run all scripts in the following order. Each script must complete successfully 
before running the next.

1. `code/processing-code/01_load_clean.qmd`
   - Output: `data/processed-data/prams_clean.rds`

2. `code/processing-code/02_create_analytic_dataset.qmd`
   - Output: `data/processed-data/prams_analytic_localfix.rds`
   - Note: prams_analytic_localfix.rds is the file used for all downstream 
     analyses and manuscript rendering. It was created to resolve a file 
     compatibility issue with the original analytic dataset.

3. `code/eda-code/03_exploratory_analysis.qmd`
   - Output: `results/figures/screening_vs_postpartum_depression.png`
   - Output: `results/tables/screening_distribution.rds`

4. `code/analysis-code/04_statistical_analysis.qmd`
   - Output: `results/tables/glm_bivariate_screened.rds`
   - Output: `results/tables/glm_multivariable_main.rds`
   - Output: `results/output/tidymodels_logistic_main.rds`

5. `code/analysis-code/05_model_validation.qmd`
   - Output: `results/tables/model_comparison.rds`
   - Output: `results/figures/roc_curve_comparison.png`

6. `quarto render products/manuscript/Manuscript.qmd`

## Note on file paths

The README lists `code/processing/` but the actual folder is 
`code/processing-code/`. All paths above reflect the actual folder names.

- `code/processing-code/01_load_clean.qmd`
- `code/processing-code/02_create_analytic_dataset.qmd`
- `code/eda-code/03_exploratory_analysis.qmd`
- `code/analysis-code/04_statistical_analysis.qmd`
- `code/analysis-code/05_model_validation.qmd`