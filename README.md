# 5050FinalProject
# Logistic Regression Analysis of Binge Drinking (STSCI 5050)

This repository contains my final project for **STSCI 5050 (Applied Regression Analysis)** at Cornell University. The project uses nationally representative survey data from the **National Survey on Drug Use and Health (NSDUH)** to analyze factors associated with adult binge drinking using survey-weighted logistic regression.

The goal of this analysis is not only statistical modeling, but careful interpretation of results in a public-health context, with appropriate handling of complex survey design.

---

## Project Overview

Binge drinking is a major public health concern linked to adverse health, social, and economic outcomes. Using NSDUH microdata, this project investigates how demographic characteristics, health status, employment, and other substance-use behaviors are associated with the probability of binge drinking among U.S. adults.

Key questions include:
- Which demographic and socioeconomic factors are most strongly associated with binge drinking?
- How do other substance-use behaviors (e.g., tobacco, marijuana, vaping) relate to binge drinking risk?
- How do results change when accounting for survey weights and complex sampling design?

---

## Data

- **Source:** National Survey on Drug Use and Health (NSDUH)
- **Population:** U.S. adults (with key exclusions applied per project scope)
- **Design:** Complex survey with stratification, clustering, and weights

To preserve data confidentiality, the raw NSDUH dataset is **not included** in this repository.

---

## Methodology

- **Outcome Variable**
  - Binary indicator of binge drinking behavior

- **Modeling Approach**
  - Survey-weighted logistic regression
  - Models estimated using the `survey` R package
  - Odds ratios and confidence intervals used for interpretation

- **Covariates Examined**
  - Sex
  - Age category
  - Self-reported health status
  - Employment status
  - Tobacco use
  - Vaping use
  - Marijuana use
  - Major depressive episode (adult)

- **Key Techniques**
  - Explicit handling of survey weights
  - Missing-value recoding based on NSDUH documentation
  - Incremental model building and interpretation
  - Focus on statistical significance *and* substantive meaning

---

## Tools & Packages

- **Language:** R  
- **Core Packages:**
  - `tidyverse`
  - `survey`
  - `MASS`
  - `janitor`
  - `skimr`
  - `scales`
- **Output:** R Markdown (PDF and HTML)

---

## Files

- `5050FinalProject.Rmd`  
  Full R Markdown analysis, including data cleaning, model estimation, and interpretation.

---

## Key Takeaways

- Binge drinking is strongly associated with both demographic characteristics and co-occurring substance use.
- Accounting for survey design meaningfully impacts coefficient estimates and inference.
- Survey-weighted regression is essential when working with nationally representative public health data.

---

## Disclaimer

This project was completed for academic purposes as part of coursework at Cornell University. Results should be interpreted in context and are not intended to make causal claims.

---

## Author

**Kimberly Bond**  
MPS Applied Statistics & Data Science, Cornell University  
