# Machine Learning Lab 9: K-Means & Hierarchical Clustering

## Objective
The objective of this practical is to implement, evaluate, and visualize unsupervised clustering algorithms—specifically **K-Means Clustering** and **Agglomerative Hierarchical Clustering**—on the Wholesale Customers Dataset, determine the optimal number of clusters using the Elbow Method and Silhouette Analysis, visualize clusters using Principal Component Analysis (PCA), and analyze hierarchical relationships using Dendrograms.

## Files
- `ML_Lab9.ipynb`: The Jupyter Notebook containing the Python code for the practical.
- `Wholesale_customers_data.csv`: The dataset containing annual spending (in monetary units) of clients across various product categories: Fresh, Milk, Grocery, Frozen, Detergents_Paper, and Delicassen, along with Channel and Region.

## Practical Steps Covered
1. **Data Loading & Inspection:**
   - Loading the dataset into a DataFrame using `pandas`.
   - Inspecting the features and data structure using `.head()`.
2. **Data Preprocessing:**
   - Selecting continuous spending features for clustering by excluding categorical columns (`Channel`, `Region`).
   - Feature scaling using `StandardScaler` to normalize the spending features to mean zero and unit variance.
3. **Optimal Cluster Selection:**
   - **Elbow Method:** Computing Within-Cluster Sum of Squares (WCSS) across cluster counts ($K = 1$ to $10$) to find the elbow curve.
   - **Silhouette Analysis:** Computing silhouette scores for $K = 2$ to $10$ to assess cluster separation and cohesion, identifying the best $K$ ($K = 3$).
4. **K-Means Clustering:**
   - Fitting the `KMeans` model with the optimal number of clusters ($K = 3$).
   - Assigning cluster labels and analyzing customer distribution across each cluster.
5. **Hierarchical (Agglomerative) Clustering:**
   - Fitting an `AgglomerativeClustering` model using Ward's minimum variance linkage (`linkage="ward"`) and Euclidean distance.
   - Assigning cluster labels and inspecting customer cluster distributions.
   - Generating tree visualizations using `scipy.cluster.hierarchy` `linkage` and `dendrogram` (both full and truncated representations).
6. **Dimensionality Reduction & Cluster Visualization with PCA:**
   - Projecting the 6-dimensional feature space down to 2 Principal Components using `PCA(n_components=2)`.
   - Analyzing the explained variance ratio and plotting 2D cluster scatter plots using Seaborn.
7. **Model Evaluation:**
   - Evaluating clustering performance using `silhouette_score`.

## Requirements
To run the notebook, ensure you have the following installed:
- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`
