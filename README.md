# EEG Seizure Detection using Convolutional Neural Networks

## Project Overview

Electroencephalography (EEG) is a non-invasive technique for recording and monitoring brain electrical activity. The EEG signals obtained provide valuable information about cognitive processes, mental states, and neurological conditions such as epilepsy. EEG plays a fundamental role as a diagnostic tool in medicine and extends to various fields, including neuroscience and biomedical engineering.

One crucial aspect of EEG study is related to the detection and prediction of epileptic seizures. According to the World Health Organization (WHO), epilepsy affects approximately 50 million people worldwide. The traditional diagnosis of epilepsy involves visual analysis, conducted by a neurologist, of hours of EEG recordings to identify electroencephalographic patterns associated with seizures. However, this process can be costly and is subject to human errors.

Faced with this challenge, researchers have been dedicated to seeking alternatives that can reduce analysis time and thus assist in more efficient diagnosis. As an alternative to this scenario, the application of artificial intelligence (AI) techniques can aid in the diagnostic process.

## Objective

The objective of our work is to propose a methodology for EEG signal classification to detect epileptic seizures. We aim to develop a model that can assist in the automated detection of seizures, reducing the burden on neurologists and improving diagnostic efficiency.

## Dataset

We used the open-source EEG dataset from Boston Children's Hospital, consisting of recordings of 198 seizures in 24 patients aged between 1.5 and 22 years. 

## Methodology

### Data Preprocessing

The data were pre-processed to remove noise and artifacts using the MNE Python library, specifically designed for neurophysiological analyses. 

### Data Transformation

The pre-processed EEG data were transformed into images to be used as input for a Convolutional Neural Network (CNN).

### Model Implementation

We implemented a 19-layer CNN in the Python language using the free Google Colaboratory platform. The model's architecture was designed to effectively capture and learn the complex patterns in the EEG data associated with epileptic seizures.

### Training and Validation

- **Training Set:** We selected 6 patients for model training using cross-validation.
- **Test Set:** The remaining 18 patients were used for individual tests to assess the model's generalization capability.
- **Training Sessions:** We conducted four training sessions using different techniques to address data imbalance. 

### Performance Metrics

Due to class imbalance that biases accuracy metrics, we considered Recall for class 1 (seizure events) as the most important metric for model selection for test data application.

## Results

- **Training Set:**
  - Average Recall for class 1: 73% (unbalanced data) and 83% (balanced data)
- **Test Set:**
  - Average Recall for class 1: 38% (unbalanced data) and 74% (balanced data)

## Limitations

Computational resources were a limiting factor, influencing the size of the training set and the variability of patterns to be learned by the network. 

## Conclusion

Despite the challenge of dealing with extreme class imbalance, our classification model achieved good performance. The results demonstrate the potential of AI techniques in aiding the diagnosis of epilepsy through automated EEG analysis.

## Future Work

Future work could focus on improving model performance by:
- Increasing the size and diversity of the training dataset.
- Utilizing more advanced data augmentation techniques.
- Exploring different neural network architectures.
- Leveraging more powerful computational resources.

## Contact

For any questions or further information, please contact me at hannacarla47@gmail.com

---


