# Cryptocurrencies
Unsupervised learning, Transformation and Clustering, PCA
## Overview of the project 
Create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. Since there is no known output for what to looking for, need to use unsupervised learning. To group the cryptocurrencies, use a clustering algorithm. Finallay, use data visualizations to share findings with the board.
## Approaches
- preprocessing (cleaning, scaling) the database,
- using Principal Component Analysis to see the data in dimentional reduction,
- clustering cryptocurrencies using K-Means algorithm,
- visualizing classified results with 2D and 3D scatter plots. 
## Resources
[Crypto_data](https://github.com/ShiraliObul/Cryptocurrencies/blob/main/crypto_data.csv)

Tools : Python, jupyter notebook, skilearn

## Results
#### Clustering Cryptocurrencies using K-Means - Elbow Curve
Using unsupervised machine learning to identify clusters of the cryptocurrencies.
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10 to define the ideal number of clusters based on data features. So, based on the Elbow curve, we will use 4 clusters to categorize the crytocurrencies. 


![Screen Shot 2022-10-01 at 10 57 21 AM](https://user-images.githubusercontent.com/65901034/193730078-f70beb14-6da8-4742-8348-c21805096784.png)

#### Visualizing Cryptocurrencies Results with hvplot (HoloViews)
##### 3D-Scatter plot with PCA algorithm to reduce the crytocurrencies dimensions to three principal components on clusters

![Screen Shot 2022-10-01 at 10 58 15 AM](https://user-images.githubusercontent.com/65901034/193730429-c54380cd-a995-469d-93ff-c1f674a8be0a.png)

#### Tradable Cryptocurrencies Table
We created hv_table as an interactive table in the jupyter notebook, as you can see in the picture below as sorted by class, most of the cryptocurrencies belongs to #0, #1 classes, and there is only one cryptocurrencies belongs to #3, which is highlight here, BitTorrent;

![Screen Shot 2022-10-03 at 11 55 51 PM](https://user-images.githubusercontent.com/65901034/193730976-7df3715b-dff8-4adb-9354-82b5030b8895.png)

#### 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply
Plotting the scatter plot with two cryptocurrency features directly does not efficiently segregate the different classes. As you seen earlier using the PCA algorithm is the right method for better visualizations. 

![Screen Shot 2022-10-01 at 11 00 07 AM](https://user-images.githubusercontent.com/65901034/193731400-035418a4-e99d-40f3-a31b-f201ceeab298.png)

## Summary
We have showed 4 clusters of cryptocurrencies after classification of 532 cryptocurrencies based on similarities of their features by unsupervised machine learning algorithms. 3D PCA plot nicely showed the 4 clusters, most of the cryptocurrencies are part of the #0, #1 clusters, 6 of them belong to #2 cluster, only 1 of them belongs to #3. Only with two cryptocurrency features (TotalCoinMined vs TotalCoinSupply) does not efficiently segregate the different classes. So, more features giving more power to classify the cryptocurrencies in this case.

**[`^        back to top        ^`](#Overview-of-the-project)**
