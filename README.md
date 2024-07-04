## EEG_Data_Analysis_for_Mental_Arithmetic_Tasks
This project is an assignment for the IIT Roorkee internship in deep learning. It involves the analysis of EEG data during mental arithmetic tasks using both traditional power spectral density (PSD) analysis and advanced neural network models: EEGNet and Vision Transformer (ViT).

# Project Overview
The aim of this project is to classify EEG data recorded during resting and mental arithmetic tasks. The analysis involves feature extraction from EEG signals, training of deep learning models, and evaluating their performance.

#Data
The dataset used in this project contains EEG recordings from 36 subjects, with each subject having two recordings: one during rest and one during a mental arithmetic task.

# Methodology
1. Data Loading and Preprocessing
EEG data is loaded using the mne library.
Only EEG channels are selected for analysis.
Power spectral density (PSD) is computed for different frequency bands: Delta, Theta, Alpha, Beta, and Gamma.
2. Feature Extraction
Features are extracted from the PSD values for each frequency band.
The extracted features are used to train the models.
3. Models
EEGNet:
- A convolutional neural network designed for EEG data classification.
- The model architecture includes multiple convolutional layers, batch normalization, dropout, and dense layers.
- The model is trained and evaluated on the extracted features.
Vision Transformer (ViT):
- EEG data is reshaped and duplicated to simulate RGB images.
- Data augmentation is applied to the reshaped data.
- ViT is used to classify the EEG data after processing it into image patches.
- The model is trained using a PyTorch DataLoader and evaluated on the test set.

# License
This project is licensed under the MIT License.

# Acknowledgements
This project is part of an internship assignment for IIT Roorkee in deep learning.
