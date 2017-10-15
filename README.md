# The Nature Conservancy Fisheries Monitoring

## Team Member 
+ Yueying Teng (yt2495@columbia.edu)
+ Pengfei Wang (pw2406@columbia.edu)
+ Kewen Zhang  (kz2246@columbia.edu)

## Introduction
This project is inspired by one competition on Kaggle.com "the-nature-conservancy-fisheries-monitoring" [Link](https://www.kaggle.com/c/the-nature-conservancy-fisheries-monitoring).

## Environments
+ Operating System: macOS Sierra
+ Language: Python2.7
+ Software: Pyspark, Opencv3

## Outline
### Train Haar-feature-based cascade classifiers
+ [detection_crop_train_fish.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/detection_crop_train_fish.py): Crop fish from pictures in the training image set
+ [detection_train_haar_classifier.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/detection_train_haar_classifier.py): Train Cascade classifier
+ [detection_generate_negative.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/detection_generate_negative.py): Generate negative instances
+ [detection_clustering_ship.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/detection_clustering_ship.py): Cluster the fishing boats 
+ [detection_crop_window.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/detection_crop_window.py): Get window location for each type of fishing boat

### Bag of Visual Words & Forest-based Classifier  
+ [classification_get_sift_bow.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/classification_get_sift_bow.py): Extract SIFT features and cluster to bags as feautres 
+ [classification_mllib_pyspark.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/classification_mllib_pyspark.py): Forest-based classifier with Pyspark


### Convolutional Neural Network
+ [classification_cnn.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/classification_cnn.py): Construct Convolutional Neural Network model
+ [classification_cnn_LAG.py](https://github.com/Sapphirine/Kaggle_the_Nature_Conservancy_Fisheries_Monitoring/blob/master/lib/classification_cnn_LAG.py): Improve result by re-weighting

## Video Presentation 
https://youtu.be/dlaS8nACQ7w

