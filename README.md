# Cryptocurrencies
## Project Overview
The purpose of this project is to analyze cryptocurrency data using Unsupervised Machine Learning. The cryptocurrency data from CryptoCompare is analysed using Pandas to fit Unsupervised Machine Learning models. A clustering algorithm is used to group data and hvPlot visualization are used to share results.
### Resources
* Data Source: Crypto_data.csv from CryptoCompare
* Software: scikit-learn 0.24, hvPlot 0.7.0, Plotly 4.14.3
## Results
### Elbow Curve
<img width="808" alt="Screen Shot 2022-10-18 at 9 53 57 PM" src="https://user-images.githubusercontent.com/107584361/196601533-4f4e8ee3-5fc6-4220-b7ab-f05d2a8bf363.png">

From the elbow curve above, it can be determined that the optimal number of clusters is 4 (k=4). This information is used for specifying the number of clusters (n_clusters) when initializing the K-means model:

`model = KMeans(n_clusters=4, random_state=0)`
### 3D-Scatter plot with clusters
<img width="777" alt="Screen Shot 2022-10-18 at 9 57 13 PM" src="https://user-images.githubusercontent.com/107584361/196602233-d282158d-bafd-43a1-8fe2-62fdda9e5be7.png">

The PCA algorithm is used to reduce the cryptocurrencies dimensions to three principal components
### hv Table
<img width="759" alt="Screen Shot 2022-10-18 at 9 55 11 PM" src="https://user-images.githubusercontent.com/107584361/196602769-46ad39e9-8253-4fcf-a7cc-9b5baf2e7b77.png">
The hvTable above displays all of the currently tradeable cryptocurrencies. This table is created using the hvplot.table() function.
### hvplot Scatter 
<img width="760" alt="Screen Shot 2022-10-18 at 9 55 59 PM" src="https://user-images.githubusercontent.com/107584361/196603036-c9a548af-dba5-4c0a-8dfc-8c9eda7a5181.png">
The graph above is a scatter plot grouped by class.
## Summary
We have identified 532 tradable cryptocurrencies using Unsupervised Machine Learning.
