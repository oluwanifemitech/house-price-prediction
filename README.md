# House Price Prediction (Ames Housing Dataset)

This repository contains a complete data science project focused on predicting house prices using the Ames Housing dataset from a Kaggle competition. The project demonstrates an end-to-end machine learning workflow, from data exploration to model tuning and final submission.

---

## Project Overview

The goal of this project is to predict the final sale price of homes in Ames, Iowa, based on 79 explanatory variables describing various aspects of residential properties. This is a classic regression problem that showcases a wide range of data science techniques.

The final, tuned XGBoost model is used to generate predictions on the test dataset, which are then formatted for submission to the Kaggle competition.

- **Data Source:** [Ames Housing Dataset on Kaggle](https://www.kaggle.com/code/alexisbcook/exercise-introduction/input)

## Key Skills Demonstrated

* **Exploratory Data Analysis (EDA):** In-depth analysis of feature distributions, correlations (using Seaborn heatmaps), and relationships between variables.
* **Data Cleaning:** Handling missing values with intelligent imputation strategies based on the data description (e.g., filling `NaN` in 'PoolQC' with 'None').
* **Feature Engineering:** Transforming skewed data (log transformation), creating new features (e.g., `TotalSF`), and converting categorical features to a numerical format (one-hot encoding).
* **Model Comparison:** Training and evaluating multiple regression models (Linear Regression, Ridge, Random Forest, Gradient Boosting, XGBoost) using robust cross-validation.
* **Hyperparameter Tuning:** Optimizing the best-performing model (XGBoost) using `RandomizedSearchCV` to maximize its predictive accuracy.

## How to Use

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```

2.  **Set up the environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Or .\venv\Scripts\activate on Windows
    pip install -r requirements.txt
    ```

3.  **Download the Data:**
    Download `train.csv` and `test.csv` from the [Kaggle competition page](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) and place them in the root of the project folder.

4.  **Run the Notebook:**
    Launch Jupyter Notebook or JupyterLab and open the `house_price_prediction.ipynb` file to see the complete analysis and code.
    ```bash
    jupyter notebook
    ```
