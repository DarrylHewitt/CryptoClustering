# Crypto Clustering

## Overview

I undertook a project utilizing Python and unsupervised learning to predict whether cryptocurrencies are influenced by 24-hour or 7-day price changes. The analysis involved clustering cryptocurrencies based on their market data using the K-means algorithm and evaluating the impact of feature reduction through Principal Component Analysis (PCA).

## Project Structure

- **CryptoClustering**
  - `Crypto_Clustering.ipynb` (Jupyter Notebook containing code)
  - `crypto_market_data.csv` (Dataset used for analysis)
  - `README.md` (This file)

## Project Execution

1. **Setup:**
   - Created a new repository for this project called `CryptoClustering`.
   - Cloned the repository to my computer.
   - Pushed the changes to GitHub.

2. **File Preparation:**
   - Renamed the `Crypto_Clustering_starter_code.ipynb` file as `Crypto_Clustering.ipynb`.
   - Loaded the `crypto_market_data.csv` into a DataFrame.
   - Obtained summary statistics and visualized the data structure.

3. **Data Preparation:**
   - Used `StandardScaler()` from scikit-learn to normalize the data.
   - Created a DataFrame with scaled data, setting "coin_id" as the index.

4. **Finding the Best Value for k Using the Original Scaled DataFrame:**
   - Utilized the elbow method to find the best value for k.
   - Answered the question: What is the best value for k?

5. **Clustering Cryptocurrencies with K-means Using the Original Scaled Data:**
   - Initialized the K-means model with the best value for k.
   - Fitted the K-means model using the original scaled DataFrame.
   - Predicted clusters and created a scatter plot using hvPlot.

6. **Optimizing Clusters with Principal Component Analysis:**
   - Performed PCA on the original scaled DataFrame.
   - Retrieved explained variance to determine the information attributed to each principal component.
   - Answered the question: What is the total explained variance of the three principal components?
   - Created a new DataFrame with PCA data, setting "coin_id" as the index.

7. **Finding the Best Value for k Using the PCA Data:**
   - Used the elbow method on the PCA data to find the best value for k.
   - Answered the question: What is the best value for k when using the PCA data? Does it differ from the best k value found using the original data?

8. **Clustering Cryptocurrencies with K-means Using the PCA Data:**
   - Initialized the K-means model with the best value for k from PCA.
   - Fitted the K-means model using PCA data.
   - Predicted clusters and created a scatter plot using hvPlot.
   - Answered the question: What is the impact of using fewer features to cluster the data using K-Means?
