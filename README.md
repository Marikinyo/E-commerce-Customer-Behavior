# E-commerce Customer Segmentation and Recommendation System

## Overview
This project segments customers into distinct groups using clustering algorithms and provides recommendations tailored to each group. It involves data preprocessing, clustering, validation, visualization, and recommendation generation.

## Key Steps
1. **Clustering:**
   - Applied KMeans clustering to segment customers.
   - Optimal number of clusters (`k`) determined using the Elbow and Silhouette methods.
   - Generated cluster labels for each customer.
   
2. **Validation:**
   - Evaluated clustering performance using:
     - Silhouette Score
     - Calinski-Harabasz Index

3. **Visualization:**
   - Used PCA and t-SNE for 2D visualization of customer clusters.

4. **Recommendation System:**
   - Analyzed clusters to generate personalized recommendations.

## How to Run
1. Clone the repository and install dependencies:
   ```bash
   pip install -r requirements.txt
   
   
## How to Run

Execute the scripts in the following order:

1. **`data_preprocessing.py`**: Preprocess the data (cleaning, feature engineering, etc.).
2. **`elbow_method_selection.py`**: Determine the optimal `k` and save it to `optimal_k.txt`.
3. **`kmeans_clustering.py`**: Apply K-means clustering and assign cluster labels to customers.
4. **`validate_clustering.py`**: Validate the clustering performance.
5. **`visualize_clusters.py`**: Visualize the clusters.
6. **`recommendations.py`**: Generate recommendations for each cluster.


## Technologies

- Python
- scikit-learn
- Pandas
- Matplotlib and Seaborn