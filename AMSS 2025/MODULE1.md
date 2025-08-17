<p align="center">
  <img src="https://github.com/user-attachments/assets/5ce5815b-f0f2-4c90-a9d6-e19e5aa01064" alt="Supervised Learning" width="700">
</p>

<h1 align="center">AMSS 2025 Module 1</h1>

## Summary of Supervised Learning Lecture

### Introduction

This overview explains the main concepts, methods, and evaluation techniques from the supervised learning lecture. It covers model basics, training, evaluation, and ensemble methods, showing how models are built, improved, and used in real applications.

### Core Concepts and Use Cases

- Learning from labeled data to map inputs to outputs. Includes classification for discrete labels and regression for continuous outputs.
- Use cases:
  - Address deliverability improvements
  - Product packaging automation
  - Agricultural grading
  - E-commerce content extraction
  - Fraud detection
  - Search personalization

- Model pipeline:
  - Collect representative data
  - Convert raw data into numerical vectors
  - Train model using loss functions and optimization
  - Predict for new data and focus on test performance

### Fundamental Components

| Part | Description |
|------|-------------|
| Model | Function mapping inputs to outputs (e.g., linear models, neural networks) |
| Loss Function | Measures prediction error (e.g., squared loss, cross-entropy) |
| Optimization | Minimizes loss (e.g., gradient descent) |
| Regularization | Controls complexity to avoid overfitting |

Training aims to reduce loss on historical data, prediction uses the learned model on new data, and generalization measures performance on unseen data.

### Model Evaluation and Validation

- Training data is for fitting the model, test data is for checking generalization
- Balance bias (too simple) and variance (too sensitive) for best results
- Avoid overfitting and underfitting with regularization
- Use cross-validation for model selection
- Grid search and random search help tune hyperparameters

### Linear Models

| Model | Description | Loss | Solution |
|-------|-------------|------|----------|
| Linear Regression | Predicts continuous values | Squared loss | Analytical or gradient descent |
| Logistic Regression | Binary classification | Cross-entropy | Gradient-based methods |
| Regularization | L1 or L2 | Reduces complexity | Improves generalization |

### Classification Models and Metrics

- Decision trees split data based on features and may need pruning
- Bagging like Random Forest reduces variance
- Boosting like AdaBoost improves accuracy
- Metrics include confusion matrix, precision, recall, F1 score, ROC AUC, precision-recall curve
- Multiclass classification uses one-vs-rest or softmax classifiers

### Regression Metrics

| Metric | Description |
|--------|-------------|
| RMSE | Square root of average squared error |
| MAPE | Average absolute error as percentage |
| R-squared | Variance explained by model |

### Advanced Topics

- Support Vector Machines with kernels for non-linear separation
- Model tuning with validation sets or cross-validation
- Clean and meaningful data improves performance
- Monitor deployed models for data drift

>[!NOTE]
>Good supervised learning models depend on proper data, correct model choice, balanced bias and variance, and careful evaluation. Whether using simple models or advanced ensembles, the goal is robust and reliable predictions.

>[!IMPORTANT]
> During Module 1, students were tasked with practicing Exploratory Data Analysis (EDA) and data visualization techniques using an Air Quality Index (AQI) dataset. You may use [this dataset from Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india/data?select=city_day.csv) or select another dataset of your choice. Apply your skills and experiment with the data in a Jupyter Notebook environment.
