# Dimensionality Reduction Techniques for Fraud Detection

## Project Overview

This project implements various dimensionality reduction techniques on a credit card transaction dataset to evaluate their performance in fraud detection. The primary goal is to compare Principal Component Analysis (PCA) with other dimensionality reduction methods in terms of accuracy, computational efficiency, and interpretability.

## Techniques Implemented

- **Principal Component Analysis (PCA)**: A widely-used technique for reducing the dimensionality of data while preserving as much variance as possible.
- **t-Distributed Stochastic Neighbor Embedding (t-SNE)**: A technique for non-linear dimensionality reduction that is particularly useful for visualizing high-dimensional data.
- **Linear Discriminant Analysis (LDA)**: A method that focuses on maximizing the separation between multiple classes.
- **Autoencoders**: A type of neural network used for learning efficient codings of the input data.

## Dataset

The dataset used in this project is a credit card transaction dataset containing features related to transaction information and labels indicating whether the transaction is fraudulent or not. The dataset can be found in the `data/` directory.

## Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/msoundappan007/dimensionality_reduction_fraud_detection.git
    cd dimensionality_reduction_fraud_detection
    ```

2. **Create and activate a virtual environment**:
    ```sh
    python -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    ```

## Usage

1. **Prepare the Data**:
    - Load the dataset from `data/credit_card_transactions.csv`.
    - Preprocess the data (e.g., normalization, handling missing values).

2. **Run Dimensionality Reduction Techniques**:
    - Execute the script `dimensionality_reduction.py` to apply PCA, t-SNE, LDA, and Autoencoders on the dataset.
    ```sh
    python dimensionality_reduction.py
    ```

3. **Evaluate Performance**:
    - Evaluate each technique's performance in terms of fraud detection accuracy, computational efficiency, and interpretability.
    - Results and metrics will be saved in the `results/` directory.

4. **Analyze Results**:
    - Review the performance comparison in `results/performance_comparison.csv`.
    - Analyze visualizations and interpretations in the `results/` directory.

## Results

- **Fraud Detection Accuracy**: Compare the accuracy of fraud detection across different dimensionality reduction techniques.
- **Computational Efficiency**: Measure the time taken and computational resources required for each technique.
- **Interpretability**: Discuss how easily the results can be interpreted in the context of fraud detection.

## Strengths and Weaknesses

### Principal Component Analysis (PCA)
- **Strengths**:
  - Reduces dimensionality while retaining most of the variance.
  - Computationally efficient.
  - Simple to understand and implement.

- **Weaknesses**:
  - Assumes linear relationships between features.
  - Less effective for non-linear data structures.
  - Principal components are not always easy to interpret.

### Other Techniques
- **t-SNE**:
  - **Strengths**: Effective for visualizing high-dimensional data in 2D or 3D.
  - **Weaknesses**: Computationally intensive and not suitable for very large datasets.

- **LDA**:
  - **Strengths**: Maximizes class separability.
  - **Weaknesses**: Assumes normal distribution and equal covariance among classes.

- **Autoencoders**:
  - **Strengths**: Can capture non-linear relationships.
  - **Weaknesses**: Requires tuning of network parameters and can be computationally expensive.

