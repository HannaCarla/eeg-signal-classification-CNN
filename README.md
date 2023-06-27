# CNN-for-EEG-Classification
This project is my dissertation work. 
I'm using the CHB-MIT Scalp EEG Database available in https://physionet.org/content/chbmit/1.0.0/
We're transforming 1D EEG segments into images and performing a binary classification for seizure detection.
The main problem with this dataset is that is highly imbalanced. In order to get the best outcome and compare results We're preparing three different models:
    model 1: imbalanced real data
    model 2: imbalanced real data + class_weight + lower threshold
    model 3: balanced data
