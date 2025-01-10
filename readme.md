# Breast Cancer Classification Project

## Introduction

Breast cancer is one of the most common types of cancer affecting women worldwide. Early detection and accurate diagnosis are crucial in improving treatment outcomes and survival rates. Breast cancer can be classified into two categories based on the nature of the tumor:

- **Benign Tumor**: A non-cancerous growth that does not spread to other parts of the body. It is usually less harmful and can often be removed without further complications.
- **Malignant Tumor**: A cancerous growth that can invade nearby tissues and spread to other parts of the body. Malignant tumors require immediate medical intervention for effective treatment.

The goal of this project is to classify breast tumors as either malignant or benign based on features extracted from fine needle aspiration (FNA) biopsies of breast masses. The dataset used consists of numerical features describing cell nuclei characteristics.

---

## Project Objective

The primary objective of this project is to:

1. Identify the top features that can best discriminate between malignant and benign tumors.
2. Perform data preprocessing, including missing value imputation and normalization.
3. Visualize the differences in feature distributions for the two classes.
4. Apply dimensionality reduction using Principal Component Analysis (PCA).
5. Build a simple classification model using the top identified features.
6. Evaluate the model using metrics like accuracy, precision, recall, and the precision-recall curve.

---

## Dataset Information

The dataset used for this project consists of:

- **32 Columns**:
  - **ID**: Unique identifier for each sample.
  - **Diagnosis**: Malignant (M) or Benign (B).
  - **30 Features**: Numerical features describing cell nuclei characteristics extracted from FNA biopsies.

### The features used for classification are:

- `texture_mean`
- `smoothness_mean`
- `concave_points_mean`
- `texture_worst`
- `smoothness_worst`
- `concave_points_worst`

---

## Requirements

- **Python 3.x**
- **Libraries**:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`

---

## Project Steps

### 1. Data Loading
- Load the dataset and handle missing values.

### 2. Feature Selection
- Identify the top discriminative features for classification.

### 3. Normalization
- Apply Min-Max scaling or Z-score transformation for feature normalization.

### 4. Visualization
- **Heatmaps** to visualize normalized data.
- **Boxplots, violin plots, and histograms** for feature distribution.

### 5. Dimensionality Reduction
- Perform PCA and generate PCA scores plots.

### 6. Modeling
- Build a simple threshold-based classifier.
- Optimize the threshold by varying it and observing accuracy changes.

### 7. Evaluation
- Calculate accuracy, precision, recall, and generate precision-recall curves.
- Discuss trade-offs between precision and recall.

---

## Results and Findings

- The **PCA plot** showed a clear separation between malignant and benign samples, indicating the features' discriminative power.
- The **top features** significantly improved classification performance.
- A balance between **precision and recall** is critical in medical diagnostics, prioritizing **recall** to avoid missing malignant cases.

---
