# Student Performance Analysis & Grade Prediction

## Overview
This project explores student academic performance and uses machine learning to predict final mathematics grades.

## Dataset
- Source: [UCI Student Performance Dataset](https://archive.ics.uci.edu/dataset/320/student%2Bperformance)
- Records analyzed: 395
- Features in the original dataset: 33
- Missing values detected: 0
- Duplicate rows detected: 0

## Technologies
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Exploratory Data Analysis
The project investigates:
- Weekly study time and final grades
- Previous class failures and final grades
- School absences and final grades
- Correlations between student attributes

## Machine Learning
Three approaches were compared using five-fold cross-validation.

| Model | Mean MAE | Mean R² |
|---|---:|---:|
| Mean baseline | 3.43 | -0.008 |
| Linear Regression | 3.32 | 0.120 |
| Ridge Regression | 3.26 | 0.152 |

Ridge Regression achieved the lowest mean absolute error among the evaluated models.

## Limitations
Prediction performance remains limited. Correlations do not establish causation, and the results apply to this dataset and evaluation setup.

## Future Improvements
- Evaluate additional regression models
- Improve model validation
- Develop an interactive Streamlit application
