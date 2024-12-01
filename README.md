# Credit Card Fraud Detection

This project addresses credit card fraud detection using a dataset with an **imbalanced distribution** of fraudulent and non-fraudulent transactions. The dataset has been normalized for the **Amount** and **Time** features to improve model performance.

## Models Used

We implemented several classification models to predict whether a transaction is fraudulent or not. Below are the models and their respective performance metrics (Precision, Recall, and F1 Score for predicting fraud):

| Model                        | Precision (Fraud) | Recall (Fraud) | F1 Score (Fraud) |
|------------------------------|------------------|----------------|------------------|
| Logistic Regression           | 0.88             | 0.70           | 0.78             |
| Decision Tree Classifier      | 0.80             | 0.74           | 0.77             |
| Random Forest Classifier      | 0.91             | 0.61           | 0.73             |
| Support Vector Machine (SVM)  | 0.79             | 0.80           | 0.79             |

### Balanced Dataset

After addressing the imbalance in the dataset, the models were retrained using the balanced data. Here are the updated performance metrics:

| Model                        | Precision (Fraud) | Recall (Fraud) | F1 Score (Fraud) |
|------------------------------|------------------|----------------|------------------|
| Logistic Regression           | 0.91             | 0.82           | 0.86             |
| Decision Tree Classifier      | 0.87             | 0.85           | 0.86             |
| Random Forest Classifier      | 0.94             | 0.79           | 0.86             |
| Support Vector Machine (SVM)  | 0.91             | 0.78           | 0.84             |

