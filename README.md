## Wine Quality Prediction

## Project Overview

This project explores the application of linear regression models to predict wine quality based on physicochemical properties.

The main goal is to investigate the relationships between wine characteristics and quality scores, compare different regression models, and evaluate their predictive performance.

## Dataset

The dataset contains physicochemical measurements of wine samples and a quality score used as the target variable.

The target variable is `quality`, while the remaining numerical features are used as predictors.

**Dataset source:** https://www.kaggle.com/datasets/yasserh/wine-quality-dataset/data

## Project Workflow

1. **Exploratory Data Analysis (EDA)** — examine feature distributions, summary statistics, and correlations.
2. **Data Preprocessing** — prepare the features for model training and apply feature scaling.
3. **Baseline Model** — establish a reference performance using `DummyRegressor`.
4. **Model Comparison** — evaluate Linear Regression, Ridge, and Lasso using cross-validation.
5. **Hyperparameter Tuning** — use `GridSearchCV` to optimize the Lasso regularization parameter.
6. **Model Evaluation** — assess the final model on a held-out test set using regression metrics and diagnostic plots.
7. **Feature Selection and Transformation** — experiment with `VarianceThreshold` and quantile-based transformations.

## Models and Techniques

- Linear Regression
- Ridge Regression
- Lasso Regression
- StandardScaler
- K-Fold and Cross-Validation
- GridSearchCV
- VarianceThreshold
- Quantile-based feature transformation

## Evaluation Metrics

The models are evaluated using:

- **MAE (Mean Absolute Error)** — measures the average absolute prediction error.
- **MSE (Mean Squared Error)** — measures the average squared prediction error.
- **R² Score** — measures how much of the target variance is explained by the model.

Actual-versus-predicted plots and residual analysis are also used to examine model performance.

## Results

The Lasso model perfomed best

| Metric | Test Set Result |
|---|---|
| MAE | 0.5073 |
| MSE | 0.4215 |
| R² | 0.3511 |

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Open the notebook in Jupyter.
4. Run the cells sequentially.

See `requirements.txt` for the required Python packages.
