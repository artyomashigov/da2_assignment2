# Data Analysis 2 - Assignment 2

Hotel-rating analysis using the Europe hotels dataset filtered to hotels in Rome.

## Objective

Estimate which factors are associated with a hotel being highly rated, comparing LPM, logit, and probit models.

## Features

- `highly_rated`: user rating greater than or equal to 4
- `premium_hotel`: 4- or 5-star hotel
- Distance from city center

## Summary

Distance from the center is negatively associated with being highly rated, while premium hotels are more likely to be highly rated. Logit and probit produce similar predictions and avoid some of the probability-range issues of the linear probability model.
