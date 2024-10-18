# Unsupervised Anomaly Detection on Hypothyroidism Dataset

## Description
This project was completed during the second semester of my Master's program (2023/24) and focuses on applying unsupervised anomaly detection techniques to a hypothyroidism dataset. The primary goal is to identify anomalous patient records using various detection methods and combine their outputs through majority voting for enhanced accuracy.

## Dataset
The dataset consists of 7,200 patient records with 21 attributes, including 15 binary and 6 continuous features. It relates to hypothyroidism, a condition caused by an underactive thyroid, affecting the body’s metabolism.

## Objectives
- Identify anomalous patient records to detect potential medical errors or unusual health conditions.
- Apply multiple unsupervised learning methods and aggregate results through majority voting.
  
## Key Steps

### Data Preparation:
- Handled duplicate entries (71 total) without removal as they likely represent true measurements.
- Continuous features were normalized, and outliers were kept for anomaly detection.

### Methods Used:
1. **K-Nearest Neighbors (KNN)**: Proximity-based algorithm that detects anomalies based on distance to neighbors.
2. **Local Outlier Factor (LOF)**: Density-based method that identifies anomalies in low-density regions.
3. **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**: Clustering algorithm that detects anomalies outside dense clusters.
4. **Principal Component Analysis (PCA)**: Reconstruction-based technique that identifies anomalies through reconstruction error in lower-dimensional space.
5. **One-Class SVM**: Support vector method that separates normal from anomalous data.

### Majority Voting:
- Combined the results of all methods, labeling records as anomalies if flagged by at least three algorithms.

## Results
- The majority voting approach identified 425 anomalies (5.9% of the dataset).
- Visualized anomalies using dimensionality reduction techniques like PCA and t-SNE for better interpretability.

## Conclusion
This project demonstrates the effectiveness of unsupervised learning methods in identifying anomalies in medical datasets. The combination of multiple algorithms through majority voting enhances the robustness of the results, offering a reliable approach to detect unusual patterns in patient data.
