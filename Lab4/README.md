# Machine Learning Lab 4: Wine Quality Analysis

## Objective
The objective of this practical is to perform exploratory data analysis (EDA), correlation study, and predictive modeling to predict wine quality based on physicochemical tests using the WineQT dataset.

## Files
- `ML_Lab4.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `WineQT.csv`: The dataset used for training and analysis, containing physicochemical features of wine variants (like acidity, sugar, chlorides, etc.) and their quality ratings.

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the data structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Data Cleaning & Preprocessing:**
   - Checking for missing values using `.isnull().sum()`.
   - Checking for duplicate records in the dataset to ensure data quality.
3. **Exploratory Data Analysis (EDA):**
   - Analyzing the distribution of the target variable (`quality`).
   - Computing and analyzing the correlation matrix to understand the linear relationships between the features and wine quality.
4. **Model Building & Evaluation:**
   - Training machine learning models to predict the quality of the wine.
   - Evaluating the predictive performance of the models.

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
