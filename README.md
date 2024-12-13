# Parkinson’s Disease Classification Using ML

## Overview

As this project infers, machine learning is applied in the classification of Parkinson’s Disease (PD) using biomedical voice analysis data. Through the analysis of the acoustic parameters derived from recorded voice samples, the goal is to develop a reliable, fast, and contactless diagnostic tool for screening and treatment of PD.

## Motivation

Parkinson’s Disease is a chronic movement disorder that affects people’s motor and non-motor systems. The timing of diagnosis is a critical factor in the treatment of the disease. Previous diagnostic techniques can sometimes be expensive, lengthy, and inaccurate. This project complements these innovations through machine learning to avoid these challenges by using voice impairments, which are known to be early symptoms of the disease.

## Key Features

- **Data Source**: The dataset used in this project is sourced from the UCI Machine Learning Repository. It contains 24 variables and 195 observations.
- **Acoustic Features**: The feature set used in the dataset includes pitch, jitter, shimmer, HNR (Harmonic-to-Noise Ratio), and nonlinear features such as RPDE (Recurrence Period Density Entropy) and DFA (Detrended Fluctuation Analysis).
- **Target Variable**: The target variable is dichotomous, indicating whether a patient has Parkinson’s Disease (1 for positive, 0 for negative).

## Project Goals

- Identify the acoustic features that are important for classifying Parkinson’s positive and negative cases.
- Ensure model reliability through cross-validation techniques and hyperparameter tuning.
- Address issues such as class imbalance and overfitting to develop a robust and reliable model.
- Demonstrate that diagnostic tools based on voice impairments can be applied to real-world human speech data for Parkinson’s Disease detection.

## Methodology

The methodology primarily focuses on understanding the dataset and its key characteristics.

- **Feature Correlation**: Feature interactions were assessed against the target variable using heatmaps. Significant features like HNR, RPDE, and DFA were identified.
- **Feature Importance**: Features were ranked by their importance to the classification model based on the derived measure of feature importance.

### Data Preprocessing

- **Handling Missing Values**: The dataset had no missing values, making the preprocessing process straightforward.
- **Feature Scaling**: Features were standardized using `StandardScaler` to normalize the spread of features, as they vary in scales.
- **Data Splitting**: The data was split into training and testing datasets with a 70:30 ratio, respectively.

### Model Development

- **Algorithm**: A Random Forest Classifier was chosen due to its stability, high accuracy, and ability to handle non-linear correlations in the dataset.
- **Hyperparameter Tuning**: Hyperparameters such as `n_estimators`, `max_depth`, and `max_features` were optimized using grid search and 5-fold cross-validation.

## Results

1. **High Accuracy**: The Random Forest Classifier demonstrated high diagnostic accuracy.
2. **Feature Insights**: Key features like HNR, RPDE, and DFA were identified as important for PD classification.
3. **Optimized Performance**: Hyperparameter tuning improved model accuracy while minimizing overfitting.

## Conclusion

This project highlights the potential of machine learning in the early diagnosis of Parkinson’s Disease using voice analysis. The Random Forest Classifier proved to be an effective model for identifying the disease based on acoustic features. Further work with larger datasets and potentially deeper models could improve the classification performance and its applicability in real-world clinical settings.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/HamzaMalhi/Parkinson-s-Disease-Classification-Using-Machine-Learning
