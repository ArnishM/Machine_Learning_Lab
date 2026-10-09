# Machine Learning Lab 6: Seeds Dataset Analysis

## Objective
The objective of this practical is to perform exploratory data analysis (EDA) and apply machine learning algorithms (such as classification or clustering) using the geometrical properties of wheat seeds.

## Files
- `ML_Lab6.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `seeds_new.csv`: The dataset used for analysis, containing measurements of geometrical properties of kernels belonging to different varieties of wheat (e.g., area, perimeter, compactness, length, width).

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the data structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Data Cleaning & Preprocessing:**
   - Checking for missing values using `.isnull().sum()`.
   - Handling any duplicates or inconsistent data records.
3. **Exploratory Data Analysis (EDA):**
   - Analyzing the distributions of the various geometrical properties.
   - Using visualizations and correlation analysis to understand the relationships between the features.
4. **Model Building & Evaluation:**
   - Applying machine learning models to categorize the wheat varieties.
   - Evaluating the models using accuracy and other appropriate evaluation metrics.

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
