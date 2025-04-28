# Titanic Survival Prediction

This repository contains simple practice notebooks for basic data analysis using Python, specifically focusing on the Titanic dataset. It includes:

- **Basic data manipulation** with pandas
- **Data visualization** using matplotlib and seaborn
- A small **Titanic survival prediction example** using logistic regression

## Files

- `01_basic_pandas.ipynb`: Practice of basic pandas usage
- `02_data_visualization.ipynb`: Simple matplotlib and seaborn graph examples
- `03_titanic_survival_analysis.ipynb`: Titanic dataset survival analysis and simple prediction using logistic regression
- `04_feature_importance.ipynb`: Feature importance analysis using Random Forest

## Environment

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Model Summary

We built a simple **logistic regression model** to predict survival on the Titanic dataset. The predictors used were:

- **Sex** (encoded as 0: male, 1: female)
- **Age** (with missing values filled by mean)
- **Pclass** (passenger class)

The model achieved an accuracy of approximately **79.3%** on the dataset.

## Confusion Matrix

| Actual / Predicted  | Predicted 0 (Died) | Predicted 1 (Survived) |
|---------------------|--------------------|------------------------|
| **Actual 0 (Died)** | 90                 | 15                     |
| **Actual 1 (Survived)** | 22              | 52                     |

### Interpretation

- The model correctly predicted 90 deaths and 52 survivors.
- Some misclassifications occurred:
  - 15 deaths were predicted as survivors.
  - 22 survivors were predicted as deaths.
  
Despite using only basic features (**Sex**, **Age**, **Pclass**), the model performed reasonably well. The next step could be improving the model with additional features or using more advanced techniques like **Random Forest** or **SVM**.

## Next Steps

1. Improve the model with more features.
2. Try different machine learning algorithms (e.g., Random Forest, Support Vector Machines).
3. Perform hyperparameter tuning to improve accuracy.


