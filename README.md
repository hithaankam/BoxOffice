# BoxOffice Revenue Prediction

This repository contains a simple machine learning project for predicting box office revenue using linear regression. The project is implemented in a Jupyter notebook and uses a movie dataset stored in `boxoffice.csv`.

## Project Contents

- `Box_Office_Revenue_Prediction_Using_Linear_Regression_in_ML.ipynb`: Main notebook demonstrating data loading, preprocessing, model training, evaluation, and visualization.
- `boxoffice.csv`: Dataset used for training and evaluating the linear regression model.

## Goal

The notebook walks through a basic regression workflow to estimate box office revenue based on movie-related features. It is intended as an educational example for how to apply machine learning to a real-world dataset.

## Method

- Load `boxoffice.csv` and perform exploratory data analysis, including feature distributions and outlier inspection.
- Encode the `genres` text column using `CountVectorizer` to convert genres into binary indicator features.
- Drop `title` and use `domestic_revenue` as the target variable.
- Split the data into training and validation sets using a 90/10 split with `random_state=22`.
- Train an `XGBRegressor` model on the processed features.
- Evaluate the model using mean absolute error on both training and validation sets.

## Results

- Training MAE: 0.2104541861999253
- Validation MAE: 0.6358190127903746

## How to Use

1. Open the notebook in Jupyter, JupyterLab, or another notebook environment.
2. Run the notebook cells sequentially.
3. Review the results and plots.

## Notes

- The notebook is designed for learning and experimentation.
- The dataset and model are intended for demonstration rather than production use.

## Requirements

- Python 3
- Jupyter Notebook or JupyterLab
- Common data science libraries such as `pandas`, `numpy`, `scikit-learn`, and `matplotlib`.
