# Used-Vehicle-ml-prediction
Machine learning project using Python to predict used-vehicle selling prices and classify whether vehicles sell within defined listing deadlines.

# Used Vehicle Price Prediction and Sale Classification

## Project Overview

This project explores how machine learning can analyse used-vehicle data and support data-driven decisions.

The project focuses on two tasks:
- **Price Prediction:** Predicting the selling price of a used vehicle using regression.
- **Sale Classification:** Predicting whether a vehicle sells within its defined listing deadline using classification.

## Objectives

- Explore and understand used-vehicle data.
- Identify and handle missing values and data quality issues.
- Prepare numerical and categorical features for machine learning.
- Build and evaluate regression and classification models.
- Compare model performance and identify suitable approaches for each task.

## Tools and Technologies

- Python
- pandas
- scikit-learn
- seaborn
- Jupyter Notebook

## Project Workflow

1. **Data Exploration:** Examine dataset structure, feature distributions, and data quality.
2. **Data Cleaning:** Handle missing values, review unusual values, and standardise categorical data where needed.
3. **Data Preparation:** Prepare numerical and categorical features for modelling.
4. **Model Development:** Train regression models for price prediction and classification models for sale outcome prediction.
5. **Model Evaluation:** Assess model performance using appropriate metrics and compare results.
6. **Conclusion:** Summarise findings, limitations, and opportunities for improvement.

## Models

### Regression
The regression task predicts vehicle selling prices. Model performance is evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)

### Classification
The classification task predicts whether a vehicle sells within its defined listing deadline. The models explored include:
- Support Vector Machine (SVM)
- Logistic Regression
- Decision Tree

Compare classification models using appropriate metrics and cross-validation where performed.

## Results

### Regression: Selling-Price Prediction

A Linear Regression model was used to predict vehicle selling prices.

| Metric | Result |
|---|---:|
| MAE | 5,084.95 |
| RMSE | 7,495.79 |
| R² Score | 0.7172 |

The model explained approximately 71.7% of the variation in selling prices on the evaluation data.

### Classification: Sale Outcome Prediction

Three models were compared: Logistic Regression, Decision Tree, and SVM, including balanced versions of Logistic Regression and SVM.

| Model | Accuracy | F1-score |
|---|---:|---:|
| Decision Tree | 71.3% | 0.536 |
| Balanced SVM | 62.9% | 0.506 |
| Balanced Logistic Regression | 58.7% | 0.513 |

**Best overall model:** Decision Tree, based on the highest accuracy and F1-score among these final comparisons.

### Class Imbalance

The dataset contained 1,776 labelled vehicles: 83.05% sold on schedule and 16.95% did not. The initial SVM predicted only the majority class, highlighting why accuracy alone is insufficient. Balanced Logistic Regression achieved better recall (58.3%) for vehicles that did not sell on schedule than Decision Tree (28.3%).

## Future Improvements

- Improve minority-class detection using class weighting or resampling.
- Apply stratified cross-validation to assess model consistency.
- Explore additional models and feature engineering.
- Evaluate performance on unseen data and investigate prediction errors.


## Key Learnings

- Preparing real-world datasets for machine learning.
- Working with numerical and categorical features.
- Applying regression and classification to different prediction problems.
- Evaluating models and comparing their performance.
- Understanding the importance of data quality and reliable evaluation.


## Author

Vishvaja Umasankar

Master's in Artificial Intelligence Design and Development  
Seneca Polytechnic, Ontario, Canada

LinkedIn: [Vishvaja Umasankar](https://linkedin.com/in/vishvaja-umasankar-52933a180)
