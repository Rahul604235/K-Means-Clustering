# K-Means-Clustering
In all the following questions, perform K-means clustering on the two input images (car.ppm
and flower.png) for K = 3 clusters. Use only Euclidean distance as the distance measure for
all iterations. Basic data units to be clustered are vectors containing pixel data, i.e., [r g b].
Perform 5 iterations of the algorithm. To visualize the output of k-means clustering, replace
each pixels in the input image with the cluster center it belongs to and display the resulting
image.


(a) Perform K-means clustering with initial cluster means as follows:
1) c_init_1- [255, 0, 0]
2) c_init_2- [0, 0, 0]
3) c_init_3- [255, 255, 255]



(b) Perform K-means clustering on both images using random initialization of cluster means.
Generate 3 random vectors of size 1*3 that are sampled from uniform distribution in [0 255]
and use them as the cluster centers to begin the K-means with. Perform K-means clustering
using N such initializations. The cost corresponding to the output of k-means clustering can
be computed as
C = summation from i to p [dist(pi; ck)]
where dist measures the Euclidean distance between a pixel color value pi and its cluster center
ck, and P refers to the total number of pixels in the image. Use N=30 (which means that
you will repeat K-means clustering with 30 different random initializations), and find the cost
corresponding to the output in each case. Among the 30 values that you got after repeatedly
running the K-means, find the output corresponding to the lowest and highest value of C.


Note:
1) In this assignment, you will be working with a color image `car.ppm'.
2) Each pixel in a color image has (R,G,B) components. The matrix containing color image
data is a 3 dimensional matrix (e.g. - height*width*3). So [img(m,n,1) img(m,n,2) img(m,n,3)]
will give the R,G,B components at (m,n) pixel respectively.
3) At the end of K-means, if any cluster turned out to be empty, use only the non-empty clusters
to display the image.
4) People with Windows machines, please install Irfanview software in order to display .ppm
files.
