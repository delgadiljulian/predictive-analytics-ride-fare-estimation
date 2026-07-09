# Predictive Modeling of Urban Ride Fares

This repository contains an applied data science project focused on the prediction of
ride fares in urban mobility platforms, using historical trip data and a combination of
statistical and machine learning models.

The project integrates Business Intelligence and supervised learning techniques to
evaluate and compare the predictive performance of linear, ensemble, and neural network
models in a real-world pricing problem.

---

## Project Overview

**Title:**  
*Predictive Modeling of Urban Ride Fares: A Machine Learning Approach*

The study analyzes ride-level data from an urban mobility platform in New York City to
model and predict trip fares based primarily on geospatial information and trip
distance.

The workflow combines data cleaning, feature engineering, exploratory analysis, and
predictive modeling to assess how different approaches perform in estimating fares with
minimal input information.

---

## Objectives

The main objectives of the project are to:

- Model the relationship between trip distance and fare amount.
- Compare traditional econometric models with modern machine learning algorithms.
- Evaluate predictive performance using out-of-sample metrics.
- Analyze the trade-off between interpretability and prediction accuracy.

---

## Key Results

- A strong and stable positive relationship is found between distance traveled and ride
  fare.
- The expanded linear regression explains approximately 70.6% of the variance in fares.
- Machine learning models significantly outperform linear specifications.
- The best-performing model is the third neural network architecture, with RMSE of
  1.9339 and MAE of 1.2592 on the official test set.
- Gradient boosting is the closest alternative, with RMSE of 1.9632 and MAE of 1.3015.
- High predictive accuracy is achieved using a small set of features, highlighting the
  effectiveness of distance-based pricing models.

---

## Methodology

The analytical workflow follows a reproducible end-to-end pipeline:

1. Data processing and feature engineering.
2. Cleaning of geospatial coordinates.
3. Distance computation using the Haversine formula.
4. Detection and removal of outliers using IQR-based filtering.
5. Exploratory analysis of fare and distance distributions.
6. Correlation analysis using Pearson and Spearman matrices.
7. Spatial visualization using scatter, density, and hexbin maps.
8. Predictive modeling with OLS, LASSO, random forest, gradient boosting, and
   feedforward neural networks.
9. Model evaluation using train-test splits, RMSE, and MAE.

---

## Dataset

The analysis uses a public dataset of Uber trips in New York City, containing
georeferenced pickup and dropoff locations and the final fare amount.

After data cleaning and filtering, the final dataset includes approximately 180,000
valid observations.

---

## Repository Structure

```text
predictive-analytics-ride-fare-estimation/
|
|-- README.md
|-- requirements.txt
`-- uber-fare-prediction-machine-learning/
    |-- data/
    |   `-- uber.csv
    |-- docs/
    |   `-- business_intelligence_final_project_guidelines.pdf
    |-- figures/
    |   |-- 1.png
    |   |-- 2.png
    |   `-- ...
    |-- report/
    |   |-- final_report.tex
    |   `-- final_report.pdf
    `-- scripts/
        `-- ride_fare_prediction_analysis.ipynb
```

---

## Reproducibility

The project can be executed locally or in Google Colab using Python 3.10 or later.

Install the main dependencies with:

```bash
pip install -r requirements.txt
```

Running `uber-fare-prediction-machine-learning/scripts/ride_fare_prediction_analysis.ipynb`
reproduces the figures, models, and results reported in
`uber-fare-prediction-machine-learning/report/final_report.pdf`.

---

## Background and References

The project builds on standard concepts from:

- Business Intelligence and predictive analytics.
- Econometric regression models.
- Ensemble learning, including random forest and gradient boosting.
- Neural networks for regression tasks.
- Urban mobility and pricing analytics.

---

## License

This repository is released under the MIT License, allowing free academic and research
use, modification, and redistribution.

---

## Author

Julián Alberto Delgadillo Marín  
M.Sc. in Applied Economics (candidate)  
University of Buenos Aires (UBA)
