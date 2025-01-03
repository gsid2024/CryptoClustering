# CryptoClustering
mod 11
his project applies K-Means clustering and Principal Component Analysis (PCA) to classify cryptocurrencies based on their price fluctuations over various timeframes. The primary goal is to group cryptocurrencies into clusters to uncover hidden patterns and trends.

Key Steps
Data Preparation:

Loaded cryptocurrency price data from a CSV file.
Standardized the data using StandardScaler to ensure all features have equal importance.
K-Means Clustering:

Used the Elbow Method to determine the optimal number of clusters (k = 4).
Performed clustering on both the original scaled data and PCA-transformed data.
Principal Component Analysis (PCA):

Reduced the dataset dimensions to three principal components, preserving ~89% of the total variance.
Created visualizations to better understand the clustering in reduced dimensions.
Cluster Visualization:

Generated scatter plots to visualize the clusters using features (price_change_percentage_24h, price_change_percentage_7d) and PCA components (PC1, PC2).
Feature Importance:

Analyzed the weights of each feature on the principal components to understand their influence.
Insights
Cryptocurrencies were grouped into 4 clusters based on their price change behaviors.
PCA helped reduce data dimensionality while retaining most of the information, improving clustering performance.
Specific price change metrics had significant influence on the clusters, such as price_change_percentage_30d and price_change_percentage_200d.
Requirements
Python Libraries: pandas, numpy, scikit-learn, matplotlib, hvplot
Conclusion
This project provides a scalable framework for clustering and analyzing cryptocurrencies based on their market behaviors, leveraging advanced techniques like PCA and K-Means. It can be extended to include additional features or used for other financial datasets.
