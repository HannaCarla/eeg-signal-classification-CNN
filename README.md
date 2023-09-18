# CNN-for-EEG-Classification
# Overview
This repository contains the code and resources for my Master's Degree project focused on EEG (Electroencephalography) classification using Convolutional Neural Networks (CNNs). The project aims to analyze EEG data and classify it into relevant categories or labels.

# Method
We're using the CHB-MIT Scalp EEG Database available in https://physionet.org/content/chbmit/1.0.0/
The database contains EEG recordings from 24 patients age 1.5 to 22 years.
We use the entire dataset. Patients 1, 2, 3, 5, 8 and 11 are used as train set and the remaining as test set to investigate the generalization capacity of our model.
## Train and Test
80% of the training data were submitted to Stratified K-Fold Cross Validaton and 20% to check for overfitting. 
The main problem with this dataset is that is highly imbalanced. In order to get the best outcome and compare results We trained and test 4 models:
    model 1: train and test with imbalanced data
    model 2: train and test with imbalanced data + class_weights + 50% threshold
    model 3: train and test with imbalanced data + class_weights + 40% threshold
    model 3: balanced data
## 1D Signal to Image
We're transforming 1D EEG segments into images to use as input to a CNN Model.


