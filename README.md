# 💳 Credit Card Fraud Detection with Logistic Regression

## 📌 Project Overview

This repository provides a step-by-step workflow for detecting fraudulent credit card transactions using Logistic Regression. The challenge lies in the highly imbalanced data—fraudulent transactions make up a tiny fraction of total transactions. To tackle this, we apply data balancing techniques and thorough feature engineering.

---

## 🛠️ Workflow

<details>
<summary>🔹 1. Data Preprocessing</summary>
✅ Loaded a large dataset (284,807 transactions, 31 features).  
✅ No missing values detected.  
✅ Features scaled (StandardScaler) for optimal model performance.  
✅ Handled severe class imbalance via **undersampling**.
</details>  

---

<details>
<summary>🔹 2. Exploratory Data Analysis (EDA) 📊</summary>
🔍 Examined class distribution: Only ~0.17% transactions are fraudulent.  
📈 Compared transaction amounts: Frauds average higher amounts ($122 vs $88).  
🔗 Feature correlations checked.
⚠️ Noted dataset is extremely imbalanced.
</details>  

---

<details>
<summary>🔹 3. Feature Engineering ⚙️</summary>
🧠 Selected relevant features based on correlation and business knowledge.  
🔢 Normalized transaction amounts and other features.
</details>  

---

<details>
<summary>🔹 4. Model Training 🤖</summary>
🏁 Built and trained a **Logistic Regression** model.  
⚖️ Used balanced data for training (undersampling).  
🔀 Employed train-test split for robust evaluation.
</details>  

---

<details>
<summary>🔹 5. Model Evaluation 📏</summary>
Evaluated using:
- ✅ **Accuracy**: ~99% (but see note below)
- ✅ **Precision**
- ✅ **Recall** (focus on fraud detection)
- ✅ **F1-Score**
- ✅ **ROC-AUC Curve**

🔥 **Special focus on Recall**: Minimizing false negatives is critical in fraud detection—catching fraud is more important than overall accuracy.

🏆 **Results (Example):**
| Metric      | Baseline (Imbalanced) | After Balancing |
|-------------|----------------------|----------------|
| Accuracy    | 99.8%                | 97.5%          |
| Recall (Fraud) | 20%                | 85%            |
| Precision   | 70%                  | 80%            |
| F1-Score    | 30%                  | 82%            |

*Note: Accuracy is high due to class imbalance. The key metric is recall for fraud cases.*

</details>  

---

## 📂 Tech Stack

- **Language**: Python 🐍
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

## 🚀 Key Takeaways

- Logistic Regression is effective for fraud detection when data imbalance is addressed.
- **Undersampling** greatly improves recall for fraudulent transactions.
- In fraud detection, recall and precision for fraud cases are more important than raw accuracy.

---

## 📈 Future Work

🔧 Apply **SMOTE** for synthetic oversampling.  
🧠 Experiment with advanced models: Random Forest, XGBoost, Neural Networks.  
🌐 Deploy model for real-time fraud detection.

---

✨ This project shows how simple algorithms, when paired with proper preprocessing and balancing, can play a vital role in financial fraud prevention.
