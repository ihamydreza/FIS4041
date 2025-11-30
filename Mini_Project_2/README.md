# Mini Project 2: Advanced Intelligent Systems - SVM and RBF Networks

This repository contains the second mini-project for the "Fundamentals of Intelligent Systems" course. This project provides a deep dive into the theoretical and practical aspects of Support Vector Machines (SVMs) and explores the application of Radial Basis Function (RBF) Neural Networks for non-linear system identification.

## 📝 Project Breakdown

The project is composed of two main sections: a thorough exploration of Support Vector Machines and an advanced implementation of RBF Networks.

### Part 1: Support Vector Machines (SVM)

This section covers the mathematical principles of SVMs from the ground up, followed by a practical implementation for a real-world classification task.

#### 1.1. Theoretical Foundations
The project begins with a detailed mathematical review of SVM theory, including:
-   **Hard-Margin SVM:** Formulation of the primal problem, derivation of the margin width, and the dual problem using Lagrange multipliers.
-   **Soft-Margin SVM:** Formulation with both **L1 (Hinge Loss)** and **L2 regularization**, analyzing the role of the `C` parameter in managing the bias-variance trade-off.
-   **Duality and KKT Conditions:** In-depth analysis of the Karush-Kuhn-Tucker (KKT) conditions and their role in identifying support vectors.
-   **Kernel Theory:** Definition of valid kernels (Mercer's Theorem) and proof of validity for **Polynomial** and **RBF kernels**.
-   **Manual Calculation:** A step-by-step manual calculation of the decision boundary and support vectors for a hard-margin SVM on a 2D dataset.

#### 1.2. Practical Implementation: Breast Cancer Classification
-   **Objective:** To classify breast cancer tumors as benign or malignant using a linear SVM.
-   **Dataset:** The Wisconsin Breast Cancer dataset.
-   **Methodology:**
    1.  **Data Preprocessing:** Loaded, cleaned, and scaled the data using `StandardScaler`.
    2.  **Visualization:** Used **Principal Component Analysis (PCA)** to project the data into a 2D space for visualization.
    3.  **Hyperparameter Tuning:** Trained multiple SVM models with different values for the `C` parameter (from 0.01 to 1000) to analyze its impact on model performance, margin size, and the number of support vectors.
    4.  **Evaluation:** Assessed the models using **Accuracy, Precision, Recall, F1-Score,** and **ROC/AUC curves**. The results demonstrate a high-performing model with an AUC score of approximately 0.99.

### Part 2: RBF Neural Networks for Non-Linear Problems

This section explores the power of RBF Networks for solving non-linear problems, culminating in a system identification task.

#### 2.1. Theoretical Analysis: RBF vs. MLP
-   An analysis of why **RBF Networks** are theoretically better suited than standard **MLP/Sigmoid networks** for classifying non-linearly separable, clustered data (e.g., the XOR problem), due to their use of local radial basis functions.

#### 2.2. Implementation: System Identification with RBFNN
-   **Objective:** To approximate the behavior of a non-linear dynamic system (a `beam and ball` model) using an RBF Network.
-   **Implementations:**
    1.  **Static RBFNN:**
        -   An RBF network with a fixed number of neurons (`K`) was implemented.
        -   Neuron centers were selected randomly from the training data.
        -   Output weights were trained in a single step using **Linear Least Squares (LLS)**.
        -   The impact of `K` (number of neurons) and `sigma` (neuron width) on RMSE was analyzed.
    2.  **Adaptive RBFNN (Inspired by M-RAN):**
        -   A more advanced, adaptive network was implemented.
        -   The network can **grow** by adding new neurons when it encounters novel data or high error.
        -   It also includes a **pruning strategy** to remove redundant neurons, aiming for an efficient network topology.
        -   This model was trained sequentially and its performance was compared to the static RBFNN.

## 📂 File Structure

All code, data, and reports for this project are organized as follows:


