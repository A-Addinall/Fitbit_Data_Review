# README

This repository contains an analysis of the relationship between sleep quality and exercise effort levels using data sourced from Fitbit devices. The primary objective is to determine the influence of sleep duration and quality on the required effort levels for subsequent workouts and establish a predictive model for daily exercise effort targets based on sleep and activity data.

## Executive Summary

The analysis aims to examine the interrelationship between sleep quality and exercise effort levels, utilizing Fitbit data. The goal is to create a predictive model that sets daily exercise effort targets based on sleep and activity data from the preceding day, optimizing workout plans by aligning them with individual rest and recovery patterns.

## Hypothesis

The hypothesis is that there exists a correlation between the exercise and sleep metrics from the previous day and the optimal effort level for exercise on the subsequent day. Specifically, better sleep quality and higher levels of exercise activity are expected to be linked to a higher recommended effort level for exercise.

## Data Collection

The data was taken from Kaggle.com (Fitbit Fitness Tracker Data) and consists of 18 datasets. After reviewing the data, a subset of data was selected, including:

- `minuteSleep_merged`: sleep state per minute
- `dailyIntensities_merged`: activity levels and time spent at each level
- `minuteMETsNarrow_merged`: 'metabolic equivalent' (MET's) score per minute

## Data Preparation

Data was prepared by converting data to the same time period, updating date formats, and merging datasets to create a final dataset.

## Data Analysis

The analysis revealed that sedentary minutes were the most prevalent among the recorded data, while very active minutes were the least common. Due to a significant proportion of missing sleep data, a decision was made to exclude sleep data from the project, resulting in a final dataset of 940 rows.

## Model Validation and Results

The predictive model exhibits strong performance in predicting future target METs scores, with a Mean Squared Error (MSE) of approximately 0.00591, R-squared (R²) score of approximately 0.927, Root Mean Squared Error (RMSE) of approximately 0.077, and Mean Absolute Error (MAE) of approximately 0.050.

## Conclusion

The analysis suggests that the predictive model effectively captures the relationship between previous day's exercise metrics and the subsequent day's effort level for exercise. Despite the removal of sleep data, the model still provides valuable insights for individuals to optimize their exercise routines based on their activity patterns.

## Recommendations

The predictive model can be utilized for predicting the target METs score for the subsequent day based on the activity metrics from the previous day, aiding in preventing overtraining and promoting optimal training regimens.

## Future Improvements

Future improvements include utilizing additional datasets, incorporating data from other fitness tracker brands, expanding the range of metrics, and considering environmental factors to offer enhanced insights and recommendations to users.
