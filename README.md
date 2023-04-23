# Predicting-Label-with-Multiple-Machine-Learning-Models

The aim of this project is to predict the top-level labels by using the code review comments questions. The research 
focuses on five different categories of top-level labels: Suggestion, Requests, Attitudes and emotions, Hypothetical 
scenario, and Rhetorical questions. The independent feature in the model is the "Question" column in the dataset, 
while the target variable is "top-level labels."

In First phase of this lab: Implement 4 models by applying preprocessing steps →
After preparing the dataset, the Random Forest algorithm is used as a benchmark model. The goal of this project is to 
enhance the model's performance, which is achieved by introducing three new machine learning models include SVM, 
XGBRFClassifier, and BaggingClassifier, to predict top-level labels. The evaluation metrics include accuracy, recall, 
and precision, by using 10-fold cross-validation.


Result: 
SVM can perform well even with small or imbalanced datasets, as it focuses on finding the best separation between 
classes rather than fitting the data closely. In this project, our dataset is small and imbalanced. In contrast, Random 
Forest may struggle with small or imbalanced datasets, as it may be overfit to the majority class and perform poorly 
on the minority classes. BaggingClassifier can use any base model, not just decision trees. SVC() is used here as base 
models. This can allow the model to use more flexible and complex base models that can better capture the underlying 
patterns in the data, which is particularly important in small datasets where the underlying patterns may not be obvious. 
BaggingClassifier with SVM base estimator may have less overfitting than Random Forest, as SVM tries to find the 
hyperplane that maximizes the margin between the classes. The XGBRFClassifier has better performance than the 
Random Forest algorithm as it can perform better in small datasets due to its ability to handle less data more 
effectively. Additionally, XGBRFClassifier uses a gradient boosting framework, which allows it to learn complex 
non-linear relationships between the features and the target variable, thus enabling it to make more accurate predictions 
than Random Forest algorithm.



