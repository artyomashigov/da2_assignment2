# Data Analysis 2 - Assignment 2

Notebook analysis of hotel ratings in Rome using the Europe hotels dataset.

## Project Overview

This assignment studies which hotel characteristics are associated with a hotel being highly rated. The dependent variable is `highly_rated`, a binary indicator equal to 1 when the user rating is 4 or higher.

The analysis compares three probability-modeling approaches: a linear probability model, a logit model, and a probit model. The notebook then compares how the models behave and visualizes their predicted probabilities.

## Research Questions

- Are hotels closer to the city center more likely to be highly rated?
- Are 4- and 5-star hotels more likely to receive high user ratings?
- How do LPM, logit, and probit estimates compare for the same classification problem?
- Do nonlinear probability models produce more reasonable predicted probability ranges than the LPM?

## Data Preparation

The notebook filters the hotels Europe dataset to focus on Rome hotels. It removes extreme distance values, keeps hotel-type accommodations, and creates binary variables for the modeling task.

Key variables:

- `highly_rated`: 1 if rating is at least 4, otherwise 0.
- `premium_hotel`: 1 if the hotel has 4 or 5 stars.
- Distance from the city center.

## Notebook Structure

- Importing libraries and data
- Cleaning and filtering the Rome hotel sample
- Creating binary target and feature variables
- Estimating a linear probability model
- Estimating a logit model
- Estimating a probit model
- Comparing predicted probabilities across models
- Visualizing model outputs
- Interpreting coefficients, confidence intervals, and model fit

## Methods

The notebook uses LPM, logit, and probit specifications. It compares coefficient direction, statistical significance, confidence intervals, predicted probabilities, R-squared or pseudo-R-squared, Brier score, and log loss.

## Key Findings

- Greater distance from the city center is associated with a lower probability of being highly rated.
- Premium hotels are substantially more likely to be highly rated.
- Logit and probit models produce very similar results.
- The nonlinear models avoid some of the LPM's probability-range issues and provide more realistic predicted probability bounds.

## Files

- `da2_assignment2_artyom-ashigov.ipynb` - full notebook with cleaning, model estimation, predictions, plots, and interpretation.
- `da2_assignment2_doc_artyom_ashigov.pdf` - exported report.

## Tools

Python, pandas, numpy, seaborn, matplotlib, plotnine, patsy, scipy, statsmodels, scikit-learn, and stargazer.
