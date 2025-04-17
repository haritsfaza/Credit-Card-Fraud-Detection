# Credit Card Fraud Detection
**Code:** [creditcard.ipynb](https://github.com/haritsfaza/credit-card-fraud-detection/blob/main/creditcard.ipynb)

**Dataset:** [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

**Goal:** The goal of this project is to automatically detect fraudulent credit card transactions based on patterns from historical data. Since the number of fraud cases is very small compared to normal transactions.

**Description:** The project focused on analyzing a dataset of credit card transactions to detect fraudulent activity. The dataset contains transactions made by European cardholders in September 2013, including anonymized features derived from PCA, transaction amount, time, and a binary fraud label. The project involved loading the data, cleaning and preprocessing it, performing exploratory data analysis (EDA), addressing class imbalance, training a Logistic Regression model, and evaluating its performance using metrics such as precision, recall, and ROC-AUC score.

**Skills:** data cleaning, data preprocessing, exploratory data analysis (EDA), handling imbalanced data, logistic regression, classification metrics, ROC-AUC analysis, confusion matrix interpretation, data visualization.

**Technology:**  Python, Pandas, Sckitlearn, Seaborn, Matplotlib.

**Results:** After preprocessing the dataset and addressing the class imbalance, a Logistic Regression model was trained using a balanced class weight configuration. The model demonstrated strong performance in detecting fraudulent transactions, achieving a recall of 0.92 on the minority class (fraud). This means that 92% of actual fraud cases were correctly identified by the model.

However, the precision was relatively low at 0.06, indicating that many of the transactions flagged as fraud were actually legitimate (false positives). Despite this, in real-world fraud detection, high recall is often prioritized to ensure minimal undetected fraud.

The model also achieved a ROC-AUC score of 0.9721, reflecting a high capability in distinguishing between fraudulent and legitimate transactions.

The confusion matrix further supports this result:
![confusion_matrix](https://github.com/user-attachments/assets/78372e13-c46c-4b53-b638-51a8c38d8613)


Only 8 fraud cases were missed (false negatives), while 1,390 normal transactions were incorrectly flagged as fraud (false positives). Overall, the model provided a strong baseline for fraud detection and can be further improved using more advanced models or resampling techniques.

