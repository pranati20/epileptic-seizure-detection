# epileptic-seizure-detection

📌 Overview
Epilepsy is a neurological disorder characterized by recurrent seizures. This project leverages Deep Learning techniques to analyze EEG (Electroencephalography) data and classify seizures in patients.

🎯 Objective
Detect epileptic seizures in EEG signals using Self-Supervised Learning (SSL).
Improve accuracy and reduce false positives in seizure detection.
Provide a scalable and automated solution for clinical applications.
📊 Dataset
Source: TUH EEG Seizure Corpus (Temple University)
Structure:
Seizure EEG samples 🟢
Non-seizure EEG samples 🔴
Multiple channels & frequencies
Preprocessing:
Noise removal (Butterworth filter)
Channel-wise normalization
Signal segmentation into time windows
🔬 Methodology
1️⃣ Data Preprocessing:

Signal filtering (bandpass, notch)
Feature extraction (FFT, Wavelet Transform)
2️⃣ Model Architecture:
CNN-RNN Hybrid: Captures spatial + temporal EEG features
Self-Supervised Learning (SimCLR/VICReg): Learns EEG representations without labeled data
3️⃣ Training & Evaluation:
Train/test split (80-20)
Cross-validation
Metrics: Accuracy, Precision, Recall, F1-score

🛠️ Tech Stack
Python (NumPy, Pandas, SciPy)
PyTorch / TensorFlow (for deep learning)
MNE-Python (for EEG signal processing)
Matplotlib & Seaborn (visualization)
