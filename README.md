## Reproducibility Instructions

This project was developed using R and Quarto. All code and outputs are organized so that the analysis can be reproduced from the raw data through the final manuscript.

### Required software
- R (version 4.x or later)
- Quarto
- R packages used in the project:
  - tidyverse
  - here
  - broom
  - knitr
  - gtsummary
  - gt

# load a few R packages
library(here)
library(knitr)

### Project structure

data/
- raw-data/ : original dataset
- processed-data/ : cleaned analytic datasets used for analysis

code/
- cleaning-code/ : scripts for data cleaning and processing
- eda-code/ : exploratory data analysis scripts
- analysis-code/ : statistical modeling scripts

results/
- figures/ : generated figures
- tables/ : processed table objects (.rds)
- output/ : model objects and saved outputs

products/
- manuscript/ : final manuscript (Quarto file and rendered HTML)
- manuscript/supplement/ : supplementary materials

### Steps to reproduce the analysis

1. Clone or download the repository.
2. Open the project in R or Positron.
3. Install required packages if needed:

```{r}
install.packages(c("tidyverse","here","broom","knitr","gtsummary","gt"))

```