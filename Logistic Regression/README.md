# Logistic Regression – Breast Cancer Classification

This project implements Logistic Regression on the Breast Cancer dataset from scikit-learn.

It includes:
- Data exploration using pandas
- Feature scaling using StandardScaler
- Train/Test split
- Model training using Logistic Regression
- Evaluation using Accuracy, Confusion Matrix, and Precision
- Understanding convergence and the effect of max_iter
- Preventing data leakage during preprocessing

---

## 📊 Dataset

We used the built-in Breast Cancer dataset from sklearn:

```python
from sklearn.datasets import load_breast_cancer

⚙️ Steps Followed

    -Load dataset and convert to pandas DataFrame.

    -Check missing values and data types using .info().

    -Split dataset into training and testing sets.

    -Apply feature scaling only on training data.

    -Train Logistic Regression model.

    -Tune max_iter to avoid convergence warnings.

Evaluate using:

    - Accuracy score is:  97.36842105263158
    - Confusion Matrix  [[41  2]
                        [ 1 70]]
    - Precision is:  0.9722222222222222

🧠 Key Learnings

    Logistic Regression is sensitive to feature scaling.

    Always split data before scaling to avoid data leakage.

    max_iter controls convergence, not accuracy.

    High accuracy does not always mean perfect generalization.

    Confusion matrix and precision give deeper insights.