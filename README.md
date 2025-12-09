# Document Clustering using TF-IDF and K-Means

## Project Overview
This project demonstrates a practical application of document clustering, a technique used to group similar text documents together. It leverages the power of TF-IDF (Term Frequency-Inverse Document Frequency) for text vectorization and the K-Means algorithm for clustering. The process also includes determining an optimal number of clusters using the elbow method and evaluating the clustering quality with the silhouette score.

## Key Steps
1.  **Data Loading**: A set of sample text documents related to Vincent Van Gogh's life are used as input.
2.  **TF-IDF Vectorization**: The text documents are converted into numerical TF-IDF vectors. This step transforms raw text into a format suitable for machine learning algorithms, highlighting important words within each document.
3.  **Optimal Cluster Determination (Elbow Method)**: The elbow method is applied to the TF-IDF matrix to identify the most suitable number of clusters (k) for the K-Means algorithm. This involves plotting the inertia (sum of squared distances of samples to their closest cluster center) against the number of clusters.
4.  **K-Means Clustering**: The K-Means algorithm is used to group the documents into the determined optimal number of clusters. Each document is assigned a cluster label.
5.  **Cluster Analysis**: The documents within each cluster are displayed to show the groupings.
6.  **Clustering Evaluation (Silhouette Score)**: The silhouette score is calculated to assess the quality of the clustering. A higher silhouette score indicates better-defined and more separated clusters.

## Libraries Used
*   `numpy`
*   `pandas`
*   `sklearn.feature_extraction.text.TfidfVectorizer`
*   `sklearn.cluster.KMeans`
*   `matplotlib.pyplot`
*   `sklearn.metrics.silhouette_score`

## How to Run
Execute the cells in sequential order within the provided Jupyter/Colab notebook. The notebook walks through each step, from data preparation to clustering and evaluation.

## Results
The project successfully demonstrates:
*   The transformation of text data into numerical representations.
*   The application of the elbow method to find an appropriate number of clusters.
*   The effective grouping of related documents using K-Means.
*   An evaluation of the clustering performance using the silhouette score.

The output includes:
*   The shape of the TF-IDF matrix.
*   An elbow curve plot to visualize inertia values.
*   Cluster assignments for each document.
*   A breakdown of documents within each cluster.
*   The calculated silhouette score for the clustering.
