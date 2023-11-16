I worked on this homework mostly by myself. I a little bit with Willow, Rayta, Chase and Christian during office hours, and a little with Miles but that's pretty much it.

This homework deals with three different methods of clustering, which are kmeans, DBSCAN, and Agglomerative Hierarchical Clustering. The goal was to find a useful model to 
cluster a set of genes based on qualities representative of numbers. kmeans is a method that picks a random amount of "centers" based on the amount of clusters you give,
finds how far each point is from each center, and assigns the point to the center closest to it. Then it finds the center of the points assigned to each cluster to find the
new "centers." The process repeats until the true center of the clusters is found. Since this dataset was basically one large blob, it did not have well defined separations
and kmeans did not work very well to make "useful" clusters. DBSCAN has two parameters, min_samples, which is the minimum number of points that need to be near a point for
it to be able to be a core point, and epsilon, which is the distance the min_points must be within in order for it to be considered "near" to the core point. Then, if any
point is within epsilon of any of the min_points, it is also considered to be in the same cluster. Any point not within epsilon of any of the points in the clusters is
considered an outlier. Since the points are all generally close together in the dataset, the DBSCAN method tended to produce one large cluster and a bunch of outliers, with
very small clusters possible depending on the epsilon and min_samples parameters chosen. Another downside to this model was that it was so sensitive to these parameters.
Agglomerative Hierarchical clustering works by starting with each point as their own cluster, and then slowly grouping points together that are closest in distance to each
other. If the closest distance is between clusters rather than individual points, it will cluster those together. This builds until there is just one large cluster. It is
hierarchical because depending on the distance between clusters, you can choose how many clusters are necessary. Due to the flexible nature of this clustering method, I
would say it was the most "useful" model for clustering the particular genes dataset we were working with. One downside though is that the distance between clusters as it
is building can be defined differently, which can drastically change the clustering. For example, in the code I did, I used ward and complete linkage methods. Ward linkage
minimizes the variance within each cluster, while complete linkage calculates the maximum distance between any two points in the clusters being merged.

The most difficult part of this assignment for me was interpreting the visualizations. I had to really delve into how the different models are made and what the different
parameters mean and how they affect the visualization and clustering. Figuring out how to standardize the data took me a bit of time as well to figure out.

The easiest part of this assignment for me was creating the visualizations. Once I researched how to code them, creating them for the dataset was easy.

One thing that I learned in this assignment was, as I stated earlier, the specifics of each of the three clustering methods and how they work to determine clusters.
