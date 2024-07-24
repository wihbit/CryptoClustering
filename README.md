# Crypto Clustering
## Summary
- An exercise in unsupervised machine learning and data preparation for ML.  
- Uses standard scaling to scale numeric data so that it has a mean of 0 and standard deviation of 1
- Uses KMeans clustering to separate cryptocurrencies into clusters, based on price change data
- Applies the elbow method to visually identify the optimal number of clusters:
    - A KMeans model is instantiated and fitted multiple times, using 1 through 10 clusters  
    - Each model's inertia ( within-cluster sum of squares) is recorded and plotted  
    - The plot shows inertia values decreasing steeply before leveling out  
    - The optimal number of clusters is visually idenitified as the point where the decrease in inertia levels out  
- Uses principal component analysis (PCA) for dimensionality reduction  
    - PCA combines the original variables into a smaller number of variables
    - PCA reduces the number of variables while retaining as much variability as possible
    - PCA1 captures the largest possible variance in the data, PCA2 captures the second largest variance, etc.
- Uses KMeans clustering again on the PCA-transformed data
