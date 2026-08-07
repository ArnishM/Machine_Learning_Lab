# Machine Learning Lab 3: Concept Learning Algorithms

## Objective
The objective of this practical is to implement two fundamental concept learning algorithms: the **Find-S Algorithm** and the **Candidate Elimination Algorithm**, to learn a target concept from a given dataset.

## Files
- `ML_Lab3.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `enjoy.csv`: The dataset used for training the algorithms. It contains features such as Sky, AirTemp, Humidity, Wind, Water, and Forecast to predict whether a sport is enjoyed (EnjoySport).

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the data structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Find-S Algorithm Implementation:**
   - Extracting features and the target variable from the dataset.
   - Initializing the most specific hypothesis.
   - Updating the hypothesis for each positive training example to find the maximally specific hypothesis.
3. **Candidate Elimination Algorithm Implementation:**
   - Initializing both specific and general boundaries.
   - Iteratively updating the specific boundary for positive examples and the general boundary for negative examples to find the version space (final specific and general boundaries).

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
