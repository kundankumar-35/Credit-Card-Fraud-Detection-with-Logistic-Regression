# 💳 Credit Card Fraud Detection with Logistic Regression

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using Logistic Regression.
Fraud detection is challenging due to the highly imbalanced dataset (fraudulent transactions are extremely rare compared to legitimate ones).
To overcome this, techniques like undersampling were applied to improve the model’s ability to correctly identify fraud.

---

## 🛠️ Workflow

<details>
<summary>🔹 1. Data Preprocessing</summary>
✅ Loaded the dataset containing credit card transactions.  
✅ Handled missing values (if any).  
✅ Scaled numerical features using StandardScaler for better model performance.  
✅ Dealt with class imbalance using undersampling.
</details>  

---

<details>
<summary>🔹 2. Exploratory Data Analysis (EDA) 📊</summary>
🔍 Checked the distribution of fraudulent vs. non-fraudulent transactions.  
📈 Visualized feature correlations using heatmaps & pair plots.  
📊 Compared transaction amounts and time distributions for both classes.  
⚖️ Observed the severe imbalance in the dataset.
</details>  

---

<details>
<summary>🔹 3. Feature Engineering ⚙️</summary>
🧩 Extracted meaningful transaction features.  
🎯 Selected important predictors based on correlation and domain relevance.  
🔄 Applied scaling & normalization for features like transaction amount.
</details>  

---

<details>
<summary>🔹 4. Model Training 🤖</summary>
🏗️ Built a Logistic Regression model.  
⚡ Trained on the balanced dataset (via undersampling).  
🧪 Used train-test split to evaluate generalization.
</details>  

---

<details>
<summary>🔹 5. Model Evaluation 📏</summary>
📊 Evaluation Metrics:  
✅ Accuracy  
✅ Precision  
✅ Recall  
✅ F1-Score  
✅ ROC-AUC Curve  

🔥 Special focus on Recall (minimizing false negatives is critical in fraud detection).  
🏆 Compared baseline (imbalanced) vs. improved (undersampled) model performance.
</details>  

---

## 📂 Tech Stack

Language: Python 🐍  
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

## 🚀 Key Takeaways

- Logistic Regression can effectively detect fraud when data imbalance is addressed.
- Undersampling significantly improved recall for fraud cases.
- Fraud detection requires prioritizing minimizing false negatives over raw accuracy.

---

## 📌 Future Work

🔧 Apply SMOTE (Synthetic Minority Oversampling Technique) for better balancing.  
🧠 Try advanced models (Random Forest, XGBoost, Neural Networks).  
📡 Deploy the model into a real-time fraud detection system.

---

✨ This project highlights how a simple yet powerful algorithm like Logistic Regression can play a vital role in detecting financial fraud when paired with proper preprocessing and balancing techniques.