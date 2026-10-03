# Machine Learning Lab 5: Diabetes Prediction Analysis

## Objective
The objective of this practical is to perform exploratory data analysis (EDA) and develop predictive models to predict the onset of diabetes based on diagnostic measures using the Diabetes dataset.

## Files
- `ML_Lab5.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `diabetes.csv`: The dataset used for training and analysis, containing various medical predictor variables (such as BMI, insulin level, age, etc.) and a target variable (`Outcome`) indicating whether the patient has diabetes.

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the data structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Data Cleaning & Preprocessing:**
   - Checking for missing values using `.isnull().sum()`.
   - Checking for duplicate records to ensure data quality.
3. **Exploratory Data Analysis (EDA):**
   - Analyzing the distributions of the medical features and the target variable (`Outcome`).
   - Performing correlation analysis to understand the linear relationships among variables.
4. **Model Building & Evaluation:**
   - Training machine learning classification models to predict the presence of diabetes.
   - Evaluating the predictive performance of the models using accuracy and other appropriate metrics.

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
