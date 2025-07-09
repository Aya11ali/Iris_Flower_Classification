# Iris Flower Classification

![MasterHead](https://www.embedded-robotics.com/wp-content/uploads/2022/01/Iris-Dataset-Classification-1024x367.png)
---

## Project Summary

**Project Description:**

The Iris Flower Classification project focuses on developing a machine learning model to classify iris flowers into their respective species based on specific measurements. Iris flowers are classified into three species: setosa, versicolor, and virginica, each of which exhibits distinct characteristics in terms of measurements.

**Objective:**

The primary goal of this project is to leverage machine learning techniques to build a classification model that can accurately identify the species of iris flowers based on their measurements. The model aims to automate the classification process, offering a practical solution for identifying iris species.

**Key Project Details:**

- Iris flowers have three species: setosa, versicolor, and virginica.
- These species can be distinguished based on measurements such as sepal length, sepal width, petal length, and petal width.
- The project involves training a machine learning model on a dataset that contains iris flower measurements associated with their respective species.
- The trained model will classify iris flowers into one of the three species based on their measurements.

---
I have selected recall as the primary evaluation metric for the Iris Flower Classification model. And after removing the overfitted models which have recall, precision, f1 scores for train as 100%, we get the final list:
| Model                     | Recall Train | Recall Test |
| ------------------------- | ------------ | ----------- |
| Logistic regression       | 0.966387     | 1.000000    |
| Logistic regression tuned | 0.974790     | 1.000000    |
| Decision Tree tuned       | 0.949580     | 0.966667    |
| Random Forest tuned       | 0.966387     | 1.000000    |
| SVM                       | 0.974790     | 1.000000    |

# 📌 Conclusion
In the Iris Flower Classification project, we applied multiple machine learning models to predict the species of Iris flowers—Setosa, Versicolor, and Virginica—based on their sepal and petal measurements. After data preparation, metric-based evaluation, and overfitting analysis, the project led to the selection of the most balanced and generalizable model.

## Data Exploration

The dataset was well-structured with no missing values. Visualizations revealed that Iris-Setosa is linearly separable from the other species, while Versicolor and Virginica had overlapping regions in feature space.

## Data Preprocessing

Since the dataset was clean and numeric, minimal preprocessing was needed. The data was split into training and testing sets, and standard scaling was applied where appropriate.

## Model Evaluation and Overfitting Detection

A wide range of models was evaluated, including Logistic Regression, Decision Trees, Random Forests, and SVMs. For each, we computed core metrics: Precision, Recall, Accuracy, F1 macro, and ROC AUC, on both train and test sets.

## Best Model Selection
Based on Recall as the primary metric (important for minimizing false negatives), the **Logistic Regression (Tuned)** model was selected. It:

* Achieved perfect Recall on the test set

* Maintained high Recall on the training set

* Showed low overfitting and strong generalization

* Is simple, interpretable, and efficient

# ✅ Final Verdict
**The Logistic Regression (Tuned)** model emerged as the optimal classifier, balancing performance and generalization. This project not only met its objectives but also introduced a reusable, clean-coded pipeline for filtering and selecting models — laying a strong foundation for similar classification tasks.

