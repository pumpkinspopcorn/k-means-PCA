# k-means-PCA

The data description mentions a dataset which contains the World Happiness Report of a total of 150 countries and the countries are arranged in an order of their respective happiness levels. There are different columns which contains the factors and attribute names that are responsible for the happiness levels of different countries mentioned. Also, an imaginary country named as Dystopia is referred which has the least happy people in the world which is needed to be compared with Utopia. We implement K-Means Clustering Algorithm and plot the features on PCA (Principal Component Axis) and perform Hierarchical Clustering and plot a dendrogram out of it with features being plotted on PCA again.

## Treatment of missing values

Detection and removal of missing values is an important step after importing the necessary libraries and dataset. No missing values were found in the data (refer the code).

## Treatment of outliers and normalisation

The next step is to plot the outliers from the columns in the dataset. Outliers are certain points in data that have values different from the others. To measure and make calculations easier for accurate results, removing them is always a better idea. After plotting the outliers, the next step is to remove the outliers. Once the outliers are removed, data normalisation is performed on it. The need for data normalisation is to rescale the values in a range between zero to one so that a common value of scale is used (refer the code).

## Determining number of clusters

Two different methods are used in this problem in determining the number of clusters present namely: Elbow Method and Silhouette Method. Both the methods are used to find the value of ‘k’ which refers to number of clusters. A cluster is a group of data which have similar values when compared it to values from all of the dataset.

![image](https://github.com/user-attachments/assets/81e218f5-e166-4bf2-acb7-bd5b43e01e00)


## Dimensional reduction using PCA

PCA is known as Principal Component Analysis which is basically a pre-processing task for preparing data for further use like for instance in this scenario, projecting the model. 
As the term says, dimensional reduction is the reduction of variables from the data so as to get a better result. In this case, dimensional reduction is done by using PCA.

## Performing k-means clustering

The basic idea of k-means clustering algorithm is to gather all the similar data in one place in a form of cluster as explained before. Centroid is used as a centre point of the clusters in the graph. After applying k-means clustering on the reduced data, we get a plotting as shown below where k=2. After performing k-means, we plot and find the centroid of it

![image](https://github.com/user-attachments/assets/1dd06334-3418-4488-93e2-999c86046e4d)

## Projection of features

Once k-means clustering is completed, projection of all the features/attributes is plotted on the PCA (Principal Component Axis). 

![image](https://github.com/user-attachments/assets/eb162e8d-72c9-4b72-8ded-bff66d052b23)

## Hierarchical clustering and plotting of dendrogram

Hierarchical Clustering is the type of clustering which groups up the similar values or objects into one which is termed as a cluster.
To show relationship between the objects or similar values, Dendrogram is used in this clustering method.
We get three clusters when we pass a horizontal line through the longest distant horizontal line in the graph. Graph down below shows the dendrogram plotted:

![image](https://github.com/user-attachments/assets/8a160739-e3ea-4541-ad3e-89f10d564f5b)

## Projection of features using hierarchical clustering

Three clusters are found and the features are projected as given below in the graph:

![image](https://github.com/user-attachments/assets/5508d9d1-6094-4a20-b195-0f3526c56f88)

## Comparison of Dystopia in contrast to Utopia

From the above graph figures E and G, it is observed that Generosity and Perception of Corruption are contributing the most as compared to other features. So, from this we can conclude that if a country has high Generosity and low Perception, it’s a Happy country as in Utopia and if a country has a low Generosity and high Perception then it’s a sad/not happy country as in Dystopia.

## Summary and Justification

In conclusion, clusters were formed for different attributes and it is observed that Social Support, Healthy Life Expectancy, Freedom to make life choices are more similar factors in determining the order of the happiest country in the world and how happy the country is.




