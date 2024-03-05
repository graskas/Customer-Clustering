# Project Overview 
In this project, I aim to conduct unsupervised clustering on customer data obtained from [Kaggle](https://www.kaggle.com/datasets/dev0914sharma/customer-clustering/data).
Customer segmentation involves categorizing customers based on shared characteristics within each cluster. By dividing customers into segments, the goal is to enhance the marketing strategies of the company according to the type of customer. This is based on the unique needs and behaviors of customers, allowing the business to address the diverse concerns of various customer types. 


## Context
The owner of a supermarket mall through membership cards,  have some basic data about your customers like Customer ID, age,sex, Marital status,Education	,Income,	Occupation	and Settlement size . The owner wants to understand the customers like who are the target customers so that the sense can be given to marketing team and plan the strategy accordingly. 

The owner of the mall have asked us to use data, and Machine Learning to help segment up their customers to aid in understanding of the customer base, and to enhance the relevancy of targeted messaging & customer communications.

## Actions

 We need to apply some data pre-processing, that is importing the relevant libraries, importing the data, and making sure that it is clean. The data was loaded using the pandas library and the first few rows were looked at using the head(). I then decided to understand the data by checking the dimension of the data and data types of variables. This allowed me to determine the data type for each variable and then also to have first look at whether there were missing values in the dataset.  The results showed that, there were no missing values. Also, since the features to look at were not given, I decided to use the top two variance to choose my features to maximize intercluster variance and minimize intra-cluster variance. 

 The data was then scaled by standardization to make sure the features are in the same scale. 
 
 
The elbow method is then used to help determine the optimal number of clusters as the K-means clustering is an unsupervised learning approach.
Based upon iterative testing using Within Cluster Sum of Squares(WCSS) and the elbow method at cluster 3, we had the WCSS to stop falling at that point (that is, we want lower WCSS or inertia errors). The Silhouette was then used to verify this results (we want a Silhouette score closer to 1) and it was between 3 clusters or 4 but 3 clusters is same as that of the Elbow method. A customer segmentation with 3 clusters was settled on. 


The data was then trained on this number of clusters to determine how customers are segmented using the KMeans algorithm.

## Conclusions
It was seen that, individuals older tend to spend more overall than those who are young. The company can bring incentives or promotional packages to individuals who are older in order to encourage them to spend more and also discount to items that are purchased by the younger ones to encourage their spending habits
