# ENERGY STAR Score Prediction Using Machine Learning

## Project Overview

This project uses machine learning to predict the ENERGY STAR Score of buildings based on building-related features.

The objective is to perform exploratory data analysis, compare multiple machine learning algorithms, and identify the best-performing regression model for predicting ENERGY STAR Scores.

## Problem Statement

The ENERGY STAR Score is a numerical measure used to assess the energy performance of eligible buildings. Predicting this score using building data can help explore patterns in building energy performance.

This project treats the task as a supervised machine learning regression problem.

## Dataset

- **Dataset Name:** Buildings energy performance data
- **Dataset :** Energy star building data.csv
- **Target Variable:** ENERGY STAR Score
- **Problem Type:** Regression

The dataset was explored, cleaned, and prepared before training and evaluating the machine learning models.

## Project Workflow

1. Data collection and loading
2. Exploratory Data Analysis (EDA)
3. Data cleaning and preprocessing
4. Feature selection and target preparation
5. Comparison of multiple regression algorithms
6. Selection of the best-performing model
7. Model evaluation on the test dataset

## Algorithms Compared

Multiple regression algorithms were evaluated, and HistGradientBoosting was selected as the final model based on the experimental results.

**Algorithms evaluated:** Linear Regression,SGD Regressor,Ridge Regressor,Lasso regressor,Decision Tree Regressor,Random Forest Regressor,
KNeighbours regressor,SVR,Gradient Boosting regressor.

## Final Model

**Selected Algorithm:** HistGradientBoosting Regressor

### Model Performance

| Metric | Test Result |
|---|---:|
| R² Score | 0.81 |
| Mean Absolute Error (MAE) | 8.95 |

- **R² = 0.81:** The model explains approximately 81% of the variation in the target values on the test dataset.
- **MAE = 8.95:** The average absolute difference between the predicted and actual ENERGY STAR Scores is approximately 8.95 points.

These results are based on the test dataset and may differ when the model is applied to new data.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn (if used)
- Scikit-learn

## How to Run the Project

1. Download or clone this GitHub repository.
2. Open the `.ipynb` notebook in Google Colab.
3. Upload the provided CSV dataset to Google Colab.
4. Update the dataset file path in the notebook if necessary.
5. Run the notebook cells in order to perform exploratory data analysis, preprocessing, model training, and evaluation.

## Repository Structure

```text
energy-star-score-prediction/
├── README.md
├── energy_star_prediction.ipynb
├── requirements.txt
└── .gitignore
```

## Conclusion

After comparing multiple regression algorithms, HistGradientBoosting was selected as the final model. It achieved an R² score of 0.81 and a Mean Absolute Error of 8.95 on the test dataset.

The notebook contains the exploratory data analysis, preprocessing steps, model comparisons, and final evaluation.

## Future Improvements

- Perform further analysis of prediction errors.
- Investigate feature importance and model interpretability.
- Evaluate generalization on additional unseen data.
