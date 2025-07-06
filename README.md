# GRP-MSc-KatellMenard-Colombia
Code used in the scope of the thesis "Interannual Growth Dynamics of Pinus patula in Mixed and Pure Stands in Medellín, Colombia" 
# 🌲 Forest Growth Modeling: Mixed and Pure Stands of *Pinus patula*

This repository contains R Markdown scripts developed for a Master's thesis on forest dynamics in tropical montane ecosystems. The study focuses on the long-term and interannual growth of *Pinus patula* in both pure and mixed-species stands, using field measurements and statistical modeling.

## 📁 Repository Structure

### `interanualOG.Rmd`
This script explores **interannual growth patterns** across four inventory years (2016, 2022, 2024, 2025). It includes:
- Tree-level and stand-level basal area (BA) calculations.
- Competition indices (Hegyi intraspecific and interspecific).
- Growth increment summaries over distinct periods.
- Histograms and summary statistics by plot and year.

### `ModMixto6.Rmd`
This script develops **nonlinear mixed-effects models** to estimate long-term diameter growth trajectories. It includes:
- Separate models for pure and mixed plots using a logistic growth function.
- A joint model with stand type as a fixed effect.
- Residual diagnostics (Shapiro-Wilk, Breusch-Pagan, Durbin-Watson).
- Model evaluation metrics (RMSE, MAPE, NSE, bias).
- Bootstrap resampling to test parameter differences.
- Visualization of observed and predicted growth curves.

## 📦 Dependencies
To run the scripts, install the following R packages:

```r
install.packages(c(
  "nlme", "dplyr", "ggplot2", "patchwork", "hydroGOF", "Metrics", "emmeans", "readxl"
))
