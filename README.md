# Predicting Label with Multiple Machine Learning Models

## About

Welcome to the "Predicting Label with Multiple Machine Learning Models" project. This project focuses on predicting top-level labels using code review comments and questions. The research centers on five distinct categories of top-level labels: Suggestion, Requests, Attitudes and emotions, Hypothetical scenario, and Rhetorical questions.

## Project Aim

The primary aim of this project is to predict top-level labels by using code review comments and questions as input data. The "Question" column in the dataset serves as the independent feature, while the target variable is the "top-level labels."

## Methodology

In the first phase of this project, we implement four machine learning models by applying preprocessing steps to the dataset. The Random Forest algorithm is initially used as a benchmark model. The goal of the project is to enhance the model's performance, which is achieved by introducing three additional machine learning models, including SVM, XGBRFClassifier, and BaggingClassifier, to predict top-level labels.

## Model Implementation

- **Random Forest**: Benchmark model.
- **SVM (Support Vector Machine)**: Robust performance even with small or imbalanced datasets.
- **XGBRFClassifier**: Offers better performance in small datasets due to its ability to handle less data more effectively.
- **BaggingClassifier**: Uses any base model, such as SVM, for better pattern capturing in small datasets.

## Evaluation Metrics

We assess model performance using the following evaluation metrics:

- **Accuracy**: Overall correctness of predictions.
- **Recall**: Ability to correctly identify positive instances (top-level labels).
- **Precision**: Ability to avoid false positive predictions.

We use 10-fold cross-validation for evaluation.

## Results

- SVM: Performs well with small or imbalanced datasets, focusing on finding the best separation between classes.
- Random Forest: May struggle with small or imbalanced datasets and overfit to the majority class.
- BaggingClassifier: Utilizes SVM as a base model, providing less overfitting and better pattern capturing.
- XGBRFClassifier: Outperforms Random Forest in small datasets, thanks to its ability to handle less data effectively and capture complex relationships between features and the target variable.

## Usage

To use this project for label prediction, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/your-username/multi-model-label-prediction.git
cd multi-model-label-prediction
