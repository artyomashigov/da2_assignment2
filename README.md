# Data Analysis 2 - Assignment 2

Hotel-rating analysis using the Europe hotels dataset filtered to hotels in Rome.

## Project Goal

The assignment estimates which hotel characteristics are associated with being highly rated. It compares a linear probability model with logit and probit models, then interprets the effect of distance from the city center and hotel quality indicators.

## Files

- `da2_assignment2_artyom-ashigov.ipynb` - full notebook with data cleaning, model estimation, prediction, and visualizations.
- `da2_assignment2_doc_artyom_ashigov.pdf` - exported report/write-up.

## Data Preparation

The notebook filters the hotels Europe dataset to Rome hotels only, removes extreme distance values, and keeps observations where the accommodation type is hotel. It creates two main binary variables:

- `highly_rated`: user rating greater than or equal to 4.
- `premium_hotel`: hotel has 4 or 5 stars.

## Methods

The analysis estimates linear probability, logit, and probit models. It compares coefficient signs, statistical significance, predicted probabilities, and model performance metrics such as log loss and Brier score.

## Key Findings

- Hotels farther from the city center are less likely to be highly rated.
- Premium hotels are more likely to receive high ratings.
- Logit and probit models produce similar predicted probabilities.
- The nonlinear models avoid some probability-range issues of the linear probability model.

## Tools

Python, pandas, statsmodels, and visualization libraries.
