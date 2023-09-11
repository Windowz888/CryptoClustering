# CryptoClustering

CryptoClustering Competition

In this analytical challenge, we use Python and unsupervised learning techniques to predict whether cryptocurrencies are affected by 24-hour or 7-day price movements. To begin, a new repository called CryptoClustering should be created. This repository should stand alone and not be merged with any other repositories. Clone this new repository to your local system when it has been created and verify that all updates are pushed to GitHub.

After cloning repository, before delving into the data, it is critical to obtain a summary of the statistics and visualize the data. The data from the CSV file should be normalized using scikit-learn's StandardScaler() module. Following normalization, a new DataFrame with the scaled data should be constructed, while retaining the old DataFrame's "coin_id" index.

Using the original scaled data, the elbow approach will be useful in determining the ideal value for k. We may visually identify the best k value by generating a line chart of all inertia values. After determining this value, the K-means model may be initialized and fitted using the original scaled DataFrame. The projected clusters for grouping the cryptocurrencies can then be displayed using hvPlot.

To further optimize our clusters, we'll do principle Component Analysis (PCA) on the original scaled DataFrame, which will reduce the features to just three principle components. We may estimate the amount of information each component contains by calculating the total explained variance of these components. The PCA data should then be used to create a new DataFrame.

The elbow approach will be crucial once more, but this time it will be applied to the PCA data to determine the ideal k value. It is critical to compare this value to the best k value discovered using the original data. The K-means model can be initiated and fitted using the optimal k value for the PCA data. Using the PCA data, predictions on the clusters for grouping the cryptocurrencies can subsequently be produced. The visualization of these clusters is possible with hvPlot. Finally, consider the implications of utilizing fewer features to cluster data with K-Means.


