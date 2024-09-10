# Credit Card Segmentation Analysis

This project performs customer segmentation on a credit card dataset using K-Means clustering. The main goal is to segment customers based on their credit card usage patterns and visualize these segments.

## Dataset

The dataset used for this analysis is the **Credit Card Data** (`CC GENERAL.csv`), which contains various attributes related to customers' credit card behavior.

### Features

- **BALANCE**: The balance left on the card at the end of the month.
- **PURCHASES**: The total amount of purchases made by the customer.
- **CREDIT_LIMIT**: The maximum limit of credit available for the customer.
- **CUST_ID**: Customer ID (dropped for analysis).

### Preprocessing Steps

1. **Remove Duplicates**: Removed any duplicate entries from the dataset.
2. **Drop CUST_ID**: The customer ID was dropped as it is not useful for clustering.
3. **Handle Missing Values**: Removed any rows with missing values.
4. **Normalization**: Applied Min-Max scaling to ensure all features are on a similar scale.

## Clustering

### K-Means Clustering

- **K-Means**: A clustering algorithm that partitions the dataset into `k` clusters. In this analysis, we chose `k=5` to create five distinct customer segments.
- The clustering was performed on the following features:
  - `BALANCE`
  - `PURCHASES`
  - `CREDIT_LIMIT`

### Cluster Mapping

The clusters were mapped to the following segments:
- **Cluster 1**
- **Cluster 2**
- **Cluster 3**
- **Cluster 4**
- **Cluster 5**

These clusters represent different customer segments based on their credit card usage behavior.

## Visualization

The clusters were visualized using a 3D scatter plot created with Plotly. The plot shows the distribution of customers across the three features (`BALANCE`, `PURCHASES`, and `CREDIT_LIMIT`) and highlights the different segments.

### 3D Scatter Plot

- **X-axis**: BALANCE
- **Y-axis**: PURCHASES
- **Z-axis**: CREDIT_LIMIT
- **Markers**: Represent different clusters (customer segments)

The interactive plot allows for exploring how different segments relate to these key features.
