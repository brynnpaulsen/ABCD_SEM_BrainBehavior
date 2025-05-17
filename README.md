# ABCD_SEM_BrainBehavior

[README (1).md](https://github.com/user-attachments/files/20260262/README.1.md)
# Cognitive Factor and Neural Network Longitudinal CFA Analysis

This project conducts confirmatory factor analysis (CFA) on behavioral and neural data across two timepoints using the ABCD dataset. It includes structural equation models, latent factor modeling, permutation tests, and difference score modeling to investigate the relationships between executive functioning (cEF), frontoparietal network (FPN), sensorimotor network (SMN), and socioeconomic adversity.

## Features
- CFA modeling of executive function and neural networks (FPN, SMN)
- Longitudinal modeling with latent difference scores
- Permutation testing to validate specificity of FPN effects
- Partial correlations and mixed effects models
- Integration with socioeconomic adversity data

## Structure
- `data/` — Place CSV input files here (e.g., `tp1_updated.csv`, `tp2_updated.csv`, `permute.csv`, `ELAdata.csv`)
- `scripts/` — Annotated R scripts for analysis
- `results/` — Place for output model summaries and statistics
- `figures/` — Any generated plots or visualizations

## Reproducibility
To reproduce:
1. Place data files in the `data/` folder.
2. Open `scripts/main_analysis.Rmd` in RStudio.
3. Run all chunks or knit to HTML.
4. Outputs will be saved in `results/`.

## Requirements
The following R packages are required:
- lavaan
- lme4, lmerTest
- tidyverse
- semTools, semPlot
- ggplot2, ggthemes, viridis, RColorBrewer
- haven, dplyr, tibble, knitr
- sjPlot, ppcor, lavaanPlot, psych, car

Use the following to install all at once:
```r
install.packages(c("lavaan", "lme4", "lmerTest", "tidyverse", "semTools", "semPlot", "ggplot2", 
                   "ggthemes", "viridis", "RColorBrewer", "haven", "dplyr", "tibble", "knitr", 
                   "sjPlot", "ppcor", "psych", "car", "lavaanPlot"))
```

## Author
This project was created by Brynn A. Paulsen, a cognitive neuroscientist studying longitudinal brain-behavior relationships.
