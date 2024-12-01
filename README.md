## Credit Card Fraud Detection

This project addresses credit card fraud detection using a dataset with an **imbalanced distribution** of fraudulent and non-fraudulent transactions. The dataset has been normalized for the **Amount** and **Time** features to improve model performance.

### Models Used

We implemented several classification models to predict whether a transaction is fraudulent or not. Below are the models and their respective performance metrics (Precision, Recall, and F1 Score for predicting fraud):

| Model                        | Precision (Fraud) | Recall (Fraud) | F1 Score (Fraud) |
|------------------------------|-------------------|----------------|------------------|
| **Logistic Regression**       | 0.83              | 0.56           | 0.67             |
| **Shallow Neural Network**    | 0.75              | 0.75           | 0.75             |
| **Random Forest Classifier**  | 0.81              | 0.47           | 0.60             |
| **Gradient Boosting Classifier** | 0.67           | 0.67           | 0.67             |
| **Support Vector Machine (SVM)** | 0.07           | 0.97           | 0.14             |

### Balanced Dataset

After addressing the imbalance in the dataset, the models were re-trained using the balanced data. Here are the updated performance metrics:

| Model                        | Precision (Fraud) | Recall (Fraud) | F1 Score (Fraud) |
|------------------------------|-------------------|----------------|------------------|
| **Logistic Regression**       | 0.93              | 0.94           | 0.94             |
| **Shallow Neural Network**    | 0.85              | 0.94           | 0.89             |
| **Random Forest Classifier**  | 1.00              | 0.51           | 0.68             |
| **Gradient Boosting Classifier** | 1.00           | 0.73           | 0.84             |
| **Support Vector Machine (SVM)** | 0.93           | 0.93           | 0.93             |

### Analysis and Observations:

- The **Shallow Neural Network** achieved a balanced performance after dataset balancing with a high F1 score of **0.89**, making it effective in fraud detection.
- **SVM** maintains excellent performance with **0.93** precision and recall, showing its strength in identifying fraud with minimal false positives.
- **Logistic Regression** also performs well with **0.94** recall and **0.93** precision, achieving an F1 score of **0.94**.
- **Random Forest** shows perfect precision (**1.00**) but lower recall (**0.51**), leading to an F1 score of **0.68**, which indicates it misses a significant amount of fraud.
- **Gradient Boosting** has high precision (**1.00**) and decent recall (**0.73**), resulting in an F1 score of **0.84**.

In conclusion, **Logistic Regression**, **SVM**, and **Shallow Neural Network** provide the best balance of precision and recall for fraud detection.


### Resources Used:
- Kaggle Dataset: [Link to the dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Tutorial: [Link to the video](https://www.youtube.com/watch?v=M_Cu7r9gik4)