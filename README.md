# Unsupervised Machine Learning and Cryptocurrency Clusters

## Overview

Machine learning is a branch of artificial intelligence wherein algorithms are used to imitate the way that humans learn to build a model that describes a data set and, ideally, gradually improves the accuracy of predictions that can be made about alternate, analogous, data sets. Machine learning can be broadly divided into the categories of “Supervised Learning” – where there is a specific outcome/output associated with the data set and the objective is to make predictions about the outcome/output associated with future data sets and “Unsupervised Learning” – where there is no specific outcome/output associated with the data set and the objective is to group the data into similar “clusters”.  Wherein data “cleaning” is often required for data analytics, when employing “Unsupervised Learning” methods it is essential to perform data “processing” to remove null values, transform any string data to numerical format and to ensure that the data has been “scaled” to reduce/eliminate any skew which might arise from variance in the size of numbers within the data set.  Once a data set has been transformed, “Unsupervised Learning” may employ “Principal Component Analysis” (PCA) to reduce the number of features in a data set being used to generate the predictive model and use of an “Elbow Curve” to assist in determining a suitable number of “clusters” into which to group the data.  The purpose of this analysis was to use the data processing requirements, K Means algorithm and PCA outlined above to generate an “Unsupervised Learning” model from data pertaining to different Cryptocurrencies for the sake of being able to place them into “clusters” or “groups” based on similarities in availability, value and performance.

## Results

Once the data had been processed to remove null values, filtered to remove entries pertaining to currencies no longer being traded and scaled to reduce skew arising from variance in the size of numbers, the data set was reduced using PCA and the K Means method was used to produce an “Elbow Curve” (See Figure 1).

### Figure 1: Elbow Curve for the Processed Cryptocurrency Data Set
![]( https://github.com/Scruffy-Bearie/Cryptocurrencies/blob/main/IMAGES/bokeh_plot.png)

Based on the “Elbow Curve” produced, the “K Means” model was applied to group the data set into 4 clusters and plotly.express was then used to produce a 3 dimensional representation of those clusters (see Figure 2).

### Figure 2: Graphical Representation of Predicted Cryptocurrency Clusters
![]( https://github.com/Scruffy-Bearie/Cryptocurrencies/blob/main/IMAGES/newplot%20(1).png)

To provide additional insights, the cryptocurrency data was also treated using the MinMaxScaler and hvplot was used to produce a plot of Total Coin Supply Vs. Total Coins Mined for the 532 tradable cryptocurrencies identified in the data set (See Figure 3).

### Figure 3: Total Coin Supply as a Function of Total Coins Mined for Tradable Cryptocurrencies
![]( https://github.com/Scruffy-Bearie/Cryptocurrencies/blob/main/IMAGES/bokeh_plot2.png)

## Analysis

The results acquired evidenced that the tradable cryptocurrencies identified in the data set could be “reasonably” placed into 4 “clusters” or groups.  Analysis indicated that one of those clusters contained only one cryptocurrency – BitTorrent  - while the remaining clusters contained a larger number of cryptocurrencies.  Additional analysis will be required to determine the exact characteristics of the clusters and the cryptocurrencies contained within before any recommendations or further conclusions can be made.
