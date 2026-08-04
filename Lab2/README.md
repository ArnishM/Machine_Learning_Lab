# Machine Learning Lab 2: Linear Regression

## Objective
The objective of this practical is to implement a **Linear Regression** model to predict house prices based on various demographic and housing features using the USA Housing dataset.

## Files
- `ML_Lab2.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `USA_Housing.csv`: The dataset used for training and testing the model. It contains features such as Average Area Income, House Age, Number of Rooms, Number of Bedrooms, and Area Population.

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Performing exploratory data analysis (EDA) using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Data Cleaning:**
   - Checking for missing values and duplicates to ensure data quality.
3. **Model Building & Evaluation:**
   - Splitting the dataset into training and testing sets using `train_test_split`.
   - Training a Multiple Linear Regression model using `scikit-learn`'s `LinearRegression`.
   - Evaluating the model's predictive performance using relevant regression metrics (such as MAE, MSE, and RMSE).

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
