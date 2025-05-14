# AI-Challenge-2025

This repository contains code and data pipelines for modeling malaria Parasite Rate (PR) across countries and years using XGBoost.

## Malaria

Malaria is a parasitic infection transmitted from person to person by the bite of infected female *Anopheles* mosquitoes. Malaria remains a global health challenge due to its high mortality rate, significant burden on healthcare systems, and potential for severe complications if untreated. You can read more about malaria [here](https://www.msf.ie/issues/malaria).

## Climate Change Is Redefining Malaria Transmission Dynamics

Floods and expanding droughts are altering the environmental conditions that support mosquito development, requiring constant adaptation of control strategies. Learn more about the impact of climate change on malaria transmission [here](https://linitiative.expertisefrance.fr/en/integrating-climate-change-into-malaria-response-in-sub-saharan-africa).

## Problem Statement

In order to limit malaria transmission, it is important to understand the key drivers of malaria parasite rate (PR). By doing so, we will be able to advise governments and global health actors on the factors they should monitor or intervene on to reduce malaria prevalence. 

This project focuses on:
- Integrating climate, health, demographic, and infrastructure indicators across countries and years.
- Building XGBoost ML models to predict malaria PR (regression).
- Identifying top contributing factors using explainable AI methods like SHAP values.

## Project Structure
<pre><code>
  ├── datasets/ # Cleaned and raw data files. Malaria_dataset.csv is the preprocessed dataset used for model training. 
  ├── script/ # R scripts for preprocessing, cleaning, training, and data analysis 
  ├── Results/ # Saved outputs 
  │ ├── XGBoost_results.rds # Saved model results 
  │ └── Graphs/ # Saved plots and SHAP visualizations 
  ├── README.md # Project overview </code></pre>

## Tools & Technologies

- **Language**: R
- **ML Frameworks**: tidymodels, xgboost
- **Visualization**: ggplot2, SHAP
- **Imputation**: No imputation was done as XGBoost model is well able to handle missing values (see [here](https://ieeexplore.ieee.org/document/9299012) )

*This repository is part of the AI Challenge 2025.*
