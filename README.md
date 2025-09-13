# Loan-Approval-Prediction
This project aims to predict loan approval status using multiple Machine Learning algorithms. The dataset includes applicant details such as income, loan amount, credit history, and demographic information.  By applying classification algorithms, we evaluate which model performs best in predicting whether a loan will be approved.


# Tech Stack

Language: Python (3.10 / 3.11 recommended)
Libraries: pandas, numpy, matplotlib, seaborn (visualization), scikit-learn (ML models, preprocessing)

# Algorithms Used & Results

| Algorithm               | Accuracy   | Notes                                   |


| ----------------------- | ---------- | --------------------------------------- |


| **Logistic Regression** | **86.17%** | High recall (0.99) for approved loans   |


| **Random Forest**       | 84.55%     | Balanced but slightly lower precision   |


| **SVM**                 | 85.36%     | Strong performance, recall 0.99         |


| **kNN**                 | **86.17%** | Performs similar to Logistic Regression |


# Results (Confusion Matrix & Report)

* Logistic Regression
Accuracy: 0.8617
Confusion Matrix: 
[[22 16]
 [ 1 84]]
High recall for loan approvals → avoids missing true approvals.

* kNN
Accuracy: 0.8617
Confusion Matrix:
[[23 15]
 [ 2 83]]
Balanced precision & recall, similar to Logistic Regression.

# Insights

Logistic Regression & kNN gave the best accuracy (86%).
SVM performed well with recall (0.99), useful in real-world scenarios where missing approvals could be costly.
Feature importance analysis (with Random Forest) can show which attributes affect loan approval most.

# Future Work

Hyperparameter tuning (GridSearchCV, RandomizedSearchCV)
Try ensemble models (XGBoost, LightGBM)
Build a Flask/Django web app for deployment
