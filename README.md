# Covid-19 case-by-case study

https://github.com/user-attachments/assets/617cf83f-d8c9-4cba-b72a-4892b3620803


## Introduction

The project performs data analysis and machine learning modeling using a Covid-19 dataset from New York City. The purpose is to analyze trends in Covid-19 cases, deaths, and hospitalizations, and predict hospitalization counts using regression models.

## Project Breakdown

1. Task 1: Exploratory Data Analysis (EDA)

    * Data Source: JSON dataset retrieved via an API endpoint.
    * Data Cleaning:
        * Dropped rows with NaN or empty values.
        * Converted date columns to datetime and extracted the month.
    * Visualization:
        * Line plots of cases, deaths, and hospitalizations over time.
        * Histogram of daily Covid-19 case counts.
        * Boxplots showing case distribution across months.

2. Task 2: Linear Regression Model

Goal: Predict hospitalization counts.
Steps:
Preprocessing:
Features selected include month, case count, and death count.
One-hot encoding for the month feature.
Split data into training and testing sets.
Trained a Linear Regression model.
Evaluation:
Measured model performance using:
Mean Squared Error (MSE)
R² score
Visualized predictions against actual hospitalization counts using scatter and line plots.
Task 3: Logistic Regression for Classification

Goal: Classify hospitalizations as "high" or "low" based on a defined threshold.
Steps:
Thresholding on hospitalization counts (e.g., 60th percentile).
Trained a Logistic Regression model.
Evaluation:
Accuracy score and classification report (precision, recall, f1-score).
Confusion matrix visualized using a heatmap.

