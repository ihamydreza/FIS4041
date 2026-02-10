# Mini Project 1: Fundamentals of Intelligent Systems

This repository contains the first mini-project for the "Fundamentals of Intelligent Systems" course. This project involves a series of exercises designed to build a strong foundation in core machine learning concepts, including classification, regression, feature selection, and dimensionality reduction.

## 📝 Project Breakdown

The project is divided into five main parts, each tackling a different aspect of machine learning.

### Part 1: Multi-Class Classification Metrics
-   **Objective:** To understand and implement key evaluation metrics from scratch.
-   **Task:** Developed the mathematical algorithm to calculate **Sensitivity** and **Specificity** for a multi-class classification problem.

### Part 2: Linear Classifiers
-   **Objective:** To implement and compare fundamental linear classification algorithms.
-   **Models Implemented:**
    1.  **Perceptron Algorithm**
    2.  **Least Squares Classifier**
    3.  **Fisher's Linear Discriminant Analysis (LDA)**
-   **Task:** Trained each model on a 2D dataset and visualized their respective decision boundaries to compare their performance.

### Part 3: The Impact of Scaling on PCA
-   **Objective:** To demonstrate the importance of data preprocessing.
-   **Task:** Provided a mathematical and practical analysis of how **Principal Component Analysis (PCA)** is sensitive to feature scaling, showing that features with larger variance can unfairly dominate the principal components if data is not scaled.

### Part 4: Customer Category Classification
-   **Objective:** To build a complete end-to-end classification pipeline.
-   **Tasks:**
    -   **Exploratory Data Analysis (EDA):** Analyzed the telecommunications customer dataset using correlation heatmaps, pair plots, and distribution charts.
    -   **Preprocessing:** Applied `StandardScaler` and `MinMaxScaler` to normalize and scale features.
    -   **Feature Selection:** Employed `Lasso (L1) Regression` and `Recursive Feature Elimination (RFE)` to identify the most impactful features.
    -   **Modeling:** Trained a `Logistic Regression` model using a One-vs-Rest (OVR) strategy for multi-class classification.
    -   **Evaluation:** Assessed model performance using Accuracy, Confusion Matrix, and ROC/AUC curves.
    -   **Dimensionality Reduction & Visualization:** Used `PCA`, `LDA`, and a custom **Multi-Layer Perceptron (MLP)** to extract and visualize features in 2D, comparing their effectiveness in separating the classes.

### Part 5: Beijing Housing Price Prediction (Regression)
-   **Objective:** To tackle a regression problem by training and comparing multiple models.
-   **Tasks:**
    -   **EDA and Preprocessing:** Analyzed the Beijing housing price dataset, identified and removed outliers using the Interquartile Range (IQR) method.
    -   **Feature Analysis:** Investigated multicollinearity between features using the **Variance Inflation Factor (VIF)**.
    -   **PCA for Regression:** Used PCA to systematically vary the number of input features and analyzed its effect on the performance (R² score) of regression models.
    -   **Comparative Model Training:** Trained and evaluated the performance of the following regression models:
        -   Multiple Linear Regression
        -   Ridge Regression
        -   Lasso Regression
        -   Polynomial Regression (demonstrating overfitting)
        -   Multi-Layer Perceptron (MLP)
        -   Elastic-Net Regression

## 📂 File Structure

The repository for this project is organized as follows:

