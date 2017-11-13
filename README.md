# Proj_CNN
# CNN project using partial Quick Draw dataset

Data source : https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap

This project uses Keras to implement a CNN model and comprises of the following parts :

(1) A CNN model which classifies images downloaded from the Quick Draw dataset. Quickdraw images used are in the 28 x 28 numpy bitmap format. Program reads all quick draw .npy files from './data_quickdraw_npy/' sub-directory, which must be downloaded from link above. Model has been trained on a downloaded quick draw sub-dataset of 40 classes with 2000 images per class. Program can accept varying number of classes (determined by the number of downloaded .npy files) and images per class can be changed by resetting global variable n_images_per_class.

(2) The model is used to predict class of objects in selected images of drawings from outside the quickdraw data set.

(3) A database of feature vectors has been compiled for the downloaded quick draw sub-dataset and saved in the sub-directory './data/'.

(4) A simple nearest image search routine based on shortest euclidean distance between the feature vector of a test image and the feature vectors from the compiled quick draw feature vector database is used to display quick draw images closest to the test image.
