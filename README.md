# ECG Arrhythmia Detection

This project implements a machine learning pipeline to detect arrhythmia from ECG signals using the MIT-BIH Arrhythmia Database. The goal is to classify ECG signals into two categories: normal and arrhythmia.

## Dataset

The dataset used in this project is the **MIT-BIH Arrhythmia Database**, which contains 48 half-hour ECG recordings of 47 different subjects. The database is widely used for training and evaluating arrhythmia detection models.

- **ECG signals**: The dataset contains ECG recordings of varying heart conditions, including both normal and arrhythmic beats.
- **Annotations**: The database also provides annotation files that mark the positions of the beats and classify them (normal, ventricular ectopic beats, etc.).

## Project Description

This project is aimed at classifying ECG signals into two categories: **normal** and **arrhythmia**.

### Key Steps in the Pipeline:
1. **Data Preprocessing**:
   - Normalization of ECG signals.
   - Creation of sliding windows of ECG signals.
   - Labeling windows based on the presence of arrhythmic events.
   
2. **Model Architecture**:
   - The model consists of multiple **1D convolutional layers** for feature extraction.
   - **MaxPooling** layers are used to reduce dimensionality.
   - Finally, a **fully connected (dense)** layer is used to make the binary classification (normal or arrhythmia).

## Setup

### Prerequisites
To run this project, you need Python 3.x and several dependencies. You can install the required packages by using the following commands:

