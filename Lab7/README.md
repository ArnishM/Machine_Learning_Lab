# Machine Learning Lab 7: Naïve Bayes Classification

## Objective
The objective of this practical is to implement and evaluate a **Naïve Bayes classifier** to classify raisin varieties (Besni and Kecimen) based on their morphological features using the Raisin Dataset.

## Files
- `ML_Lab7.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `Raisin_Dataset.xlsx`: The dataset containing morphological measurements of 900 raisin grains from two varieties — **Besni** and **Kecimen** — with features such as Area, MajorAxisLength, MinorAxisLength, Eccentricity, ConvexArea, Extent, and Perimeter.

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the data structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Data Preprocessing:**
   - Encoding the categorical target variable (`Class`) using `LabelEncoder`.
   - Splitting the dataset into training and testing sets using `train_test_split`.
   - Feature scaling using `StandardScaler`.
3. **Model Building — Gaussian Naïve Bayes:**
   - Training a `GaussianNB` classifier from `scikit-learn` on the training data.
4. **Model Evaluation:**
   - Evaluating the classifier using accuracy, precision, recall, and F1-score.
   - Generating a detailed `classification_report` and visualizing the `confusion_matrix`.

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
