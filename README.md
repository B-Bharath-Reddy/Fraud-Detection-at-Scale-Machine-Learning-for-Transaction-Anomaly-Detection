# Fraud-Detection-at-Scale-Machine-Learning-for-Transaction-Anomaly-Detection



## 📌 Overview
This project focuses on detecting fraudulent transactions using machine learning, specifically the **Isolation Forest** algorithm. The model aims to identify anomalies in financial transactions without prior knowledge of fraudulent cases, making it a powerful unsupervised learning approach.

## 🚀 Objective
- Develop an anomaly detection model to detect fraudulent transactions.
- Compare the model's performance with a **naive baseline approach** based on transaction amounts.
- Evaluate the effectiveness of the **Isolation Forest** model using **AUC-ROC**.
  
## 📊 Dataset
The dataset contains financial transaction records with features such as:
- **Amount** of the transaction
- **Balance before & after transactions** for both origin and destination accounts
- **Transaction type** (Cash In, Cash Out, etc.)
- **Timestamp (Step)** indicating the transaction hour

## 🛠️ Feature Engineering
- Derived features such as **balance changes** for both sender and receiver.
- Extracted **hour of the day** from timestamps.
- Applied **one-hot encoding** to categorical transaction types.

## 🏆 Model Approach
### 🔍 Isolation Forest
- A tree-based anomaly detection algorithm that isolates outliers effectively.
- Assigns **anomaly scores** to each transaction.
- Provides a continuous anomaly score, allowing flexible fraud detection.

### 📌 Baseline Comparison
- Compared Isolation Forest results against a **naive threshold-based method** using transaction amounts.
- Transactions with abnormally high amounts were flagged using the **isFlaggedFraud** column.
- Evaluated model performance against the **isFraud** column (ground truth labels).

## 📈 Evaluation
- Computed **AUC-ROC** to assess model effectiveness.
- The **Isolation Forest model outperformed** the naive approach, achieving an **AUC score of 0.875**.
- Identified **top anomalies** in the dataset based on anomaly scores.

## 🔥 Key Takeaways
✔️ **Unsupervised fraud detection** using Isolation Forest  
✔️ **Feature engineering** improves anomaly detection  
✔️ **Comparison with baseline approach** demonstrates model superiority  
✔️ **AUC-ROC of 0.875**, indicating strong fraud detection capability  

