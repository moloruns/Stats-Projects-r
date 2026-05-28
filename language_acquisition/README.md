# English Proficiency & Language Acquisition: A Statistical Analysis

## Overview
This report investigates predictors of English proficiency using data from Hartshorne, 
Tenenbaum & Pinker (2018), a large-scale study of over 600,000 second language learners 
who completed an online grammar test. Specifically, we examine the effects of age of 
acquisition, multilingual status, and self-reported psychiatric diagnosis on proficiency 
outcomes.

## Dataset
Data sourced from Hartshorne, Tenenbaum & Pinker (2018). The dataset contains over 
130,000 observations after cleaning, with logit-transformed grammar test scores as the 
primary outcome variable.

## Methods
- Exploratory data analysis with distribution auditing (Grubbs test) and visualization
- Inferential testing: Welch t-tests, one-way ANOVA with Tukey post-hoc, bootstrapped 
  confidence intervals
- Generalized Additive Modeling (GAM) with thin-plate splines to capture non-linear 
  acquisition-age effects
- 10-fold cross-validation for out-of-sample model comparison
- Bootstrap validation of spline stability

## Requirements
R with the following packages: `tidyverse`, `stringr`, `outliers`, `psych`, `gridExtra`, 
`effectsize`, `boot`, `mgcv`, `ggcorrplot`

## Usage
Open `language_acquisition_jup.ipynb` in Jupyter with an R kernel and run cells sequentially. 
Run the package installation cell first if packages are not already installed.
