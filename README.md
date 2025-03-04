# Ethereum Anomaly Detection

## 1. Introduction

Ethereum is one of the most widely used blockchain networks, with a vast number of transactions occurring daily. Identifying anomalous transactions is crucial for fraud detection, security monitoring, and overall network integrity. This project applies Isolation Forest for anomaly detection in Ethereum transaction data.

## 2. Dataset Description

The dataset contains Ethereum transaction records, including multiple features related to transaction amounts, addresses, timestamps, and other metadata. The data has been preprocessed for missing values and standardized before applying machine learning techniques.

## 3. Data Preprocessing

Handling Missing Values: Missing values were identified and imputed using appropriate strategies such as mean imputation or removal where necessary.

Feature Scaling: Standardization was applied to ensure uniform feature distributions, improving the performance of anomaly detection models.

Dimensionality Reduction: Principal Component Analysis (PCA) and t-SNE were used to reduce dimensionality while preserving essential patterns in the data.

## 4. Anomaly Detection Using Isolation Forest

Isolation Forest Algorithm: This unsupervised learning technique isolates anomalies by randomly selecting features and partitioning the data.

Training the Model: The Isolation Forest model was trained on the preprocessed Ethereum transaction data to learn patterns of normal transactions and identify outliers.

Prediction: The model assigned an anomaly score to each transaction, labeling those with high scores as anomalies.

Evaluation: Results were analyzed using precision-recall metrics, ROC curves, and visualization techniques.

## 5. Results & Analysis

The t-SNE visualization showed clear clusters of normal and anomalous transactions.

The model successfully detected suspicious transactions with reasonable accuracy.

Performance metrics indicate that the Isolation Forest method effectively captures anomalies with minimal false positives.

## 6. Conclusion

This project demonstrates the effectiveness of Isolation Forest in detecting anomalies in Ethereum transactions. By preprocessing the data, applying dimensionality reduction, and training an unsupervised anomaly detection model, we successfully identified fraudulent or unusual activities.
