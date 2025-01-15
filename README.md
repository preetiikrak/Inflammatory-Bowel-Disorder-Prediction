# Gene Expression Analysis for Inflammatory Bowel Disease (IBD) Prediction

This project leverages gene expression and clinical data to predict Inflammatory Bowel Disease (IBD) status using a deep learning model. The model integrates genomic features and patient-specific clinical data to classify patients as either IBD-positive or IBD-negative.

## Overview

This notebook performs the following tasks:
- Preprocessing IBD-specific gene expression and clinical data.
- Building a multi-input neural network for binary classification (IBD vs. non-IBD).
- Training the model and evaluating its performance based on accuracy and AUC metrics.
- Visualizing the training and validation process.

## Dependencies

- Python 3.x
- TensorFlow/Keras
- Pandas
- Scikit-learn
- Matplotlib
- NumPy

## Steps

1. **Data Preprocessing**:
   - Load gene expression and patient clinical data related to IBD.
   - Normalize the data and split it into training and testing sets.

2. **Model Design**:
   - The neural network has two input branches: one for gene expression data and another for patient clinical data.
   - The branches are merged and connected to an output layer for binary classification (predicting IBD status).

3. **Training and Evaluation**:
   - Compile the model using the Adam optimizer and binary cross-entropy loss.
   - Train the model with early stopping to avoid overfitting.
   - Evaluate the model on test data, and output accuracy and AUC for the IBD prediction task.

4. **Visualization**:
   - Plot the training and validation loss, accuracy, and AUC over the epochs to track model performance.

## Results

The model successfully predicted IBD status with the following performance:
- **Accuracy**: 0.946 
- **AUC**: 0.986

## Usage

To replicate or extend this work:
1. Clone the repository.
2. Install the necessary dependencies.
3. Run the notebook using IBD-specific gene expression and clinical datasets.

