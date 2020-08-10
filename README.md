Approach to the Problem :

Data is taken and features are extracted using the VGGnet16 Pre Trained model on Imagenet.
The shape of images are changed to 224x224 to feed to the VGGnet.
Based on the Features extracted from these images using VGGnet , we cluster them into different clusters using K-Means.
For the value of K , Silhouette Score is used as there can be multiple points in the Elbow method which leads to confusion.
Images are clustered based on the appropriate K.
Based on the Clustering different folders are made with images belonging to a particular cluster in the particular folder.
First Approach:
In the first approach we take an input and number of images needed as input as using kmans find the cluster the image belongs to and then just give random images from that Folder of the Cluster..
Second Approach :
In the second approach we train a resnet on the images obtained from clustering . After that we use resnet to predict the cluster of that image and randomly extract n images from that cluster folder.
