In this challenge Python and unsupervised learning was used to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.  Loaded the crypto_market_data.csv into a DataFrame and plot to review.  Used the StandardScaler() module from scikit-learn to normalize the data from the csv file.  Once the data was scaled a new DataFrame was created with the "coin_id" index brought in from the original DataFrame.

Next the best value for K was found using the original scaled DataFrame and utilizing the elbow method.  From there the clusters were predicted with K-means using the scaled data.  After a new DataFrame was completed a scatter plot was created to visualize the results.

In addition the original scaled DataFrame was used to perform PCA and reduce the features to three principal components.  The total explained variance was 88.9% of the three principal components.  A new DataFrame was created with the PCA data and the "coin_id" index from the orignial data was set.  The elbow method was used to find the best K-value to initialize the k-means and finally create a scatter plot to visualize the results.

It was discovered that using 3 features with the PCA method as opposed to 2 features with Kmeans lead to more clear clustering results.
