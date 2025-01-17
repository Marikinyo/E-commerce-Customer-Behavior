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

Execute the notebooks in the following order:

1. **`1_Clustering.ipynb`**: Determine optimal `k` and save it to `optimal_k.txt`.
2. **`2_KMeans.ipynb`**: Assign cluster labels to customers.
3. **`3_Validation.ipynb`**: Validate the clustering performance.
4. **`4_Visualization.ipynb`**: Visualize the clusters.
5. **`5_Recommendation.ipynb`**: Generate recommendations for each cluster.

## Technologies

- Python
- scikit-learn
- Pandas
- Matplotlib and Seaborn