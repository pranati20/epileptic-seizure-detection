**Epileptic Seizure Detection Using Deep Learning on EEG Data**

**Overview**
This project uses deep learning techniques to analyze EEG (Electroencephalography) data and classify seizure events. It aims to provide an automated and scalable solution for seizure detection in clinical applications.

**Objective**
Detect epileptic seizures from EEG signals using self-supervised learning (SSL).
Improve detection accuracy and reduce false positives.
Develop a model that can be integrated into real-world medical applications.

**Dataset**
Source: TUH EEG Seizure Corpus (Temple University)
**Structure:**
Seizure EEG samples
Non-seizure EEG samples
Multiple channels and frequencies

**Preprocessing Steps:**
Noise removal using a Butterworth filter
Channel-wise normalization
Segmentation into fixed time windows

**Methodology**
1. Data Preprocessing
Apply signal filtering (bandpass, notch filters)
Extract features using Fast Fourier Transform (FFT) and Wavelet Transform
Normalize EEG signals and segment data

2. Model Architecture
Use a CNN-RNN hybrid to capture spatial and temporal EEG features
Train a self-supervised learning model (SimCLR/VICReg) for feature representation

4. Training and Evaluation
Train-test split (80-20)
Apply cross-validation
Evaluate using accuracy, precision, recall, and F1-score
