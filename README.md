# Mall Customers Clustering using K-Means

This project demonstrates the implementation of K-Means clustering on a dataset of mall customers to group them based on their annual income and spending score.

---

## Table of Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Dataset](#dataset)
- [Implementation](#implementation)
- [Visualization](#visualization)
- [Results](#results)
- [Usage](#usage)
- [Author](#author)
- [License](#license)

---

## Introduction
K-Means is an unsupervised learning algorithm used for clustering. This project applies the algorithm to customer data to identify distinct groups of customers based on their income and spending behavior. These clusters can help businesses tailor their strategies to target specific customer segments.

---

## Requirements
Ensure the following Python libraries are installed:
- **Python 3.x**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Scikit-learn**

## Dataset
The dataset used in this project is the Mall Customers dataset. It contains the following columns:

CustomerID: Unique identifier for each customer
Gender: Gender of the customer
Age: Age of the customer
Annual Income (k$): Annual income of the customer in thousands of dollars
Spending Score (1-100): Spending behavior score
Ensure the dataset is saved as Mall_Customers.csv in the correct directory.

## Implementation
The code is divided into the following steps:

Import Libraries:
Necessary libraries for data manipulation, visualization, and machine learning are loaded.

Load Dataset:
The dataset is read into a Pandas DataFrame for analysis.

Feature Selection:
The features Annual Income and Spending Score are selected as inputs for clustering.

Elbow Method:
The elbow method is used to determine the optimal number of clusters. This is done by plotting the Within-Cluster Sum of Squares (WCSS) for different cluster counts.

Train K-Means Model:
The K-Means algorithm is applied with the optimal number of clusters determined in the previous step.

Cluster Visualization:
The customer clusters are visualized in a scatter plot with cluster centroids.

## Visualization
1. Elbow Method
The elbow method helps identify the optimal number of clusters by plotting the WCSS against the number of clusters. The "elbow point" on the graph indicates the best number of clusters.


2. Customer Clusters
The scatter plot below visualizes the clusters of customers. Each color represents a distinct cluster, and the yellow points mark the centroids.

## Results
Optimal Clusters
Using the elbow method, the optimal number of clusters is determined to be 5.

Cluster Insights
The clusters represent distinct customer segments:

Cluster 1 (Blue): High income, low spending.
Cluster 2 (Red): High income, high spending.
Cluster 3 (Green): Moderate income, moderate spending.
Cluster 4 (Pink): Low income, high spending.
Cluster 5 (Cyan): Low income, low spending.
## Usage
The identified clusters can help businesses:

Customize marketing strategies.
Improve customer satisfaction by understanding customer behavior.
Optimize resource allocation for targeted marketing campaigns.


Install the required libraries using:
```bash
pip install numpy pandas matplotlib scikit-learn
