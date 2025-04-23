# Deep Learning Project - Speech Emotion Recognition

## Project Overview

This project develops a deep learning-based system for accurately recognizing seven distinct emotions—anger, disgust, fear, happiness, neutral, sadness, and surprise—from speech signals.

## Data Preparation

### Datasets
We used multiple publicly available datasets:
- **RAVDESS**
- **CREMA-D**
- **TESS**
- **SAVEE**

These datasets were combined to create a comprehensive training set, enhancing the model’s generalizability.

### Data Integration
- Dataset merging and preprocessing into a unified CSV file for streamlined feature extraction.

## Data Exploration

- Conducted exploratory analysis to assess emotion distribution.
- Visualized audio signals and Mel Spectrograms for initial data insights.

## Data Augmentation
Applied several techniques to improve model robustness:
- **Noise addition:** Simulated background noises.
- **Pitch shifting:** Altered vocal pitch.
- **Time shifting:** Modified timing of speech segments.
- **Time stretching:** Adjusted playback speed without affecting pitch.

## Feature Extraction
Extracted features include:
- **Mel-Frequency Cepstral Coefficients (MFCCs):** Captures spectral properties.
- **Zero Crossing Rate (ZCR):** Measures frequency of signal crossing zero amplitude.
- **Root Mean Square Energy (RMSE):** Represents signal energy.

## Model Training
- **Convolutional Neural Network (CNN)** architecture for effective emotion classification.
- Implemented batch normalization, dropout layers, and max-pooling for regularization and generalization.
- Optimized using Adam optimizer with categorical cross-entropy loss.

## Training Performance
- Achieved training accuracy of approximately 98% and validation accuracy of around 94%.
- Applied callbacks such as Model Checkpoint, Early Stopping, and Learning Rate Reduction for efficient training.

## Model Evaluation
- Test set accuracy reached 94.39%.
- Confusion matrix and classification report indicated high precision, recall, and F1-score across all emotion classes, showcasing strong overall performance.

## Results Visualization
- Plotted training and validation accuracy/loss to evaluate model convergence.
- Created confusion matrix heatmap for detailed error analysis and model interpretability.

## Future Improvements
- Exploration of more sophisticated neural network architectures (e.g., Transformer-based models).
- Integration of additional datasets to further enhance model accuracy and generalizability.
