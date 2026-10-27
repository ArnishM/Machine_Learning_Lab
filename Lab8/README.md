# Machine Learning Lab 8: Support Vector Machines (SVM) & Hyperparameter Tuning

## Objective
The objective of this practical is to implement, evaluate, and fine-tune **Support Vector Machines (SVM)** for binary classification (predicting `Machine failure`) on the AI4I 2020 Predictive Maintenance Dataset using both Linear and RBF kernels, along with hyperparameter optimization via `GridSearchCV`.

## Files
- `ML_Lab8.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `ai4i2020.csv`: The AI4I 2020 Predictive Maintenance Dataset containing 10,000 records with features such as Air temperature, Process temperature, Rotational speed, Torque, Tool wear, machine Type, and failure indicators.

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the data structure using `.head()`, `.tail()`, `.shape`, `.info()`, and `.describe()`.
2. **Data Preprocessing & Feature Engineering:**
   - Dropping non-predictive identifiers (`UDI`, `Product ID`) and specific failure modes (`TWF`, `HDF`, `PWF`, `OSF`, `RNF`) to focus on the binary target `Machine failure`.
   - Splitting data into features ($X$) and target ($y$), followed by train-test split using `train_test_split`.
   - Constructing a `ColumnTransformer` with `StandardScaler` for numerical features and `OneHotEncoder` for categorical features (`Type`).
3. **Model Building & Evaluation — Linear SVM:**
   - Training a Linear SVM (`SVC(kernel='linear')`) via `Pipeline`.
   - Evaluating predictions with accuracy, precision, recall, F1-score, `classification_report`, and confusion matrix heatmap.
4. **Model Building & Evaluation — RBF Kernel SVM:**
   - Training a Non-linear SVM (`SVC(kernel='rbf')`).
   - Evaluating metrics, plotting confusion matrix, and comparing performance between Linear SVM and RBF SVM.
5. **Hyperparameter Tuning with GridSearchCV:**
   - Setting up a grid of hyperparameters exploring different kernels (`linear`, `rbf`), regularization parameter $C$, and kernel coefficient $\gamma$ (`gamma`).
   - Executing 5-fold cross-validation with `scoring="f1"`.
   - Extracting and analyzing the best parameters and optimal cross-validation F1-score.

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
