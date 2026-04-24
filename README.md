# Breast Cancer Detection

## Overview
This project focuses on predictive modeling for diagnosing breast cancer using machine learning techniques. The goal is to accurately predict whether a tumor is malignant or benign based on diagnostic measurements from digitized images of fine needle aspirates (FNA) of breast masses.

## Dataset
- **Dataset Name**: Breast Cancer Wisconsin (Diagnostic) Dataset
- **Description**: Comprises detailed medical measurements extracted from FNA images of breast masses, capturing features such as radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension.
- **Attributes**: 569 rows × 32 attributes
- **Label**: `diagnosis` — M (malignant) or B (benign)
- **Missing Values**: None
- **Source**: [Breast Cancer Wisconsin Dataset on Kaggle](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)

## Challenges
- **Class Imbalance**: The dataset has a majority of benign samples, requiring oversampling strategies.
- **Data Sensitivity**: Medical data requires careful handling and preprocessing.
- **Feature Selection**: With 30 diagnostic features, dimensionality reduction is important.
- **Limited Samples**: Only 569 data points, making overfitting a concern.

## Analysis Overview

1. **Exploratory Data Analysis (EDA)**: Distribution of features, correlation analysis, and visualization of diagnostic measurements.
2. **Data Preprocessing**: Handling outliers, encoding labels, and scaling numerical features.
3. **Model Training**: Logistic regression, random forests, XGBoost, and support vector machines (SVM).
4. **Model Evaluation**: Accuracy, precision, recall, F1-score, and ROC-AUC metrics.

## Explainability Methods
Feature importance analysis, SHAP (SHapley Additive exPlanations), and LIME (Local Interpretable Model-agnostic Explanations) are used to interpret model predictions and understand feature contributions.

## Installation

```bash
pip install -r requirements.txt
```

## Running the Notebook

Open `pipeline.ipynb` in Jupyter or VS Code and run all cells.

## References
- Breast Cancer Wisconsin (Diagnostic) Data Set — [Kaggle](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)
- Lundberg & Lee (2017). A Unified Approach to Interpreting Model Predictions — [arXiv](https://arxiv.org/abs/1705.07874)
- Ribeiro et al. (2016). "Why Should I Trust You?" — [arXiv](https://arxiv.org/abs/1602.04938)
