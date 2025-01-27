# E-commerce Customer Segmentation and Similarity Matrices

## Overview
This project segments e-commerce customers into distinct groups using clustering algorithms (KMeans) and generates similarity matrices for each cluster. These matrices identify customers with similar demographic and transactional characteristics, such as age, spending patterns, purchase frequency, and satisfaction levels, enabling customer segmentation for more personalized marketing strategies and improving engagement through targeted groups based on demographic and transactional data. The project involves key steps like data preprocessing, clustering, evaluation, and visualization, culminating in the generation of similarity matrices that can be used to make data-driven decisions.


### Age Group Categorization
The users were categorized into the following age ranges:

| Age Group             | Age Range |
|-----------------------|-----------|
| **Child**             | 0 - 16    |
| **Young Adults**      | 17 - 30   |
| **Middle-aged Adults**| 31 - 45   |
| **Old-aged Adults**   | 46+       |



These categories were used to segment users for clustering and to personalize recommendations based on their age groups.

### Satisfaction Levels:
The satisfaction levels are measured on a scale from 0 to 1, with the following categories:

| **Very Dissatisfied** | **Dissatisfied** | **Satisfied** | **Very Satisfied** |
|-----------------------|------------------|---------------|--------------------|
| **0**                 | **0.3**          | **0.7**       | **1**              |


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

4. **Similarity Matrices:**
   - Analyzed clusters to generate similarity matrices.

## How to Run
1. Clone the repository and install dependencies:
   ```bash
   pip install -r requirements.txt
   
### Execute the scripts in the following order:

1. **`data_preprocessing.py`**: Preprocess the data (cleaning, feature engineering, etc.).
2. **`elbow_method_selection.py`**: Determine the optimal `k` and save it to `optimal_k.txt`.
3. **`kmeans_clustering.py`**: Apply K-means clustering and assign cluster labels to customers.
4. **`validate_clustering.py`**: Validate the clustering performance.
5. **`visualize_clusters.py`**: Visualize the clusters.
6. **`Cluster Data Extraction and Analysis.py`**: Extract the clusters
7. **`similarity_matrices.py`**: Generate similarity matrices for each cluster.


## Technologies

- Python
- scikit-learn
- Pandas
- Matplotlib and Seaborn