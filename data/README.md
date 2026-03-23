# Data

This folder contains all datasets used in the project, including raw and processed data.

## Structure

- `raw-data/`  
  Original PRAMS data and supporting documentation. These files are not modified.

- `processed-data/`  
  Cleaned and analysis-ready datasets created from the raw data.

## Workflow

1. Raw data are stored in `raw-data/`
2. Data cleaning and processing are performed using scripts in:
   - `code/processing/`
3. Processed datasets are saved in `processed-data/`
4. These processed datasets are used for analysis and modeling in:
   - `code/analysis/`

## Notes

- The raw data should remain unchanged to ensure reproducibility.
- All transformations are documented in the processing scripts.
- Processed datasets include derived variables used in statistical analysis.