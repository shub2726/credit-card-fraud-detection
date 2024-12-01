## Credit Card Fraud Detection

This project addresses credit card fraud detection using a dataset with an **imbalanced distribution** of fraudulent and non-fraudulent transactions. The dataset has been normalized for the **Amount** and **Time** features to improve model performance.

### Models Used

We implemented several classification models to predict whether a transaction is fraudulent or not. Below are the models and their respective performance metrics (Precision, Recall, and F1 Score for predicting fraud):

| Model                        | Precision (Fraud) | Recall (Fraud) | F1 Score (Fraud) |
|------------------------------|-------------------|----------------|------------------|
| **Logistic Regression**       | 0.88              | 0.70           | 0.78             |
| **Random Forest Classifier**  | 0.91              | 0.61           | 0.73             |
| **Gradient Boosting Classifier** | 0.85           | 0.94           | 0.89             |
| **Support Vector Machine (SVM)** | 0.93           | 0.93           | 0.93             |

### Balanced Dataset

After addressing the imbalance in the dataset, the models were retrained using the balanced data. Here are the updated performance metrics:

| Model                        | Precision (Fraud) | Recall (Fraud) | F1 Score (Fraud) |
|------------------------------|-------------------|----------------|------------------|
| **Logistic Regression**       | 0.91              | 0.82           | 0.86             |
| **Random Forest Classifier**  | 0.94              | 0.79           | 0.86             |
| **Gradient Boosting Classifier** | 0.85           | 0.94           | 0.89             |
| **Support Vector Machine (SVM)** | 0.91           | 0.78           | 0.84             |

### Analysis and Observations:

- **Random Forest** and **Gradient Boosting** perform well on the **balanced dataset**, with strong precision and recall values.
- **SVM** achieves **very high precision and recall**, showing it is effective in catching frauds without many false positives.
- The **Logistic Regression** model performed well before balancing, but after balancing, it improved further in recall, making it more sensitive to fraud detection.

In conclusion, **SVM** and **Random Forest** models show great promise for fraud detection, particularly in balancing precision and recall.
