# supervised_fashion_cluster

SUMMARY

Project Summary: Fashion Image Clustering using CNN and K-Means

This project focuses on grouping fashion images using Convolutional Neural Networks (CNN) and K-Means clustering. The dataset contains grayscale images of clothing items, with each image represented by pixel values. First, the data is preprocessed by normalizing the pixel values to a range of 0 to 1 and reshaping them into a 28×28×1 format suitable for CNN input.

Next, a CNN model is built and trained with labeled data. The model includes convolutional layers for feature extraction, pooling layers for reducing dimensions, and dense layers for classification. Instead of using the final classification output, features are extracted from the second to last layer of the CNN. These features capture important patterns like edges, shapes, and textures learned from the images.

The extracted feature vectors are then used as input for the K-Means clustering algorithm. This algorithm groups similar images based on the closeness of their features. Since K-Means is an unsupervised learning method, it does not use labels during clustering. To visualize the results, Principal Component Analysis (PCA) reduces the high-dimensional feature space to two dimensions. A scatter plot shows how the images are grouped into clusters.

The results indicate that similar fashion items are often grouped together, although some overlap occurs due to similarities between certain classes. This project demonstrates that combining supervised feature extraction with unsupervised clustering can effectively analyze and group image data.
