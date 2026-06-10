# Customer Churn Prediction & Retention Analytics

📉 **Predict customer churn using machine learning to optimize retention strategies and safeguard recurring business revenue.**

---

## 👥 Project Team & Course Information

| Course & Term | Team | Project Contributors |
| :--- | :--- | :--- |
| AD571 – SPR 2026 | Team 1 | Antara Sudhir, Hye Won Kim, Julie Tran |

---

## 📌 Project Overview
Customer attrition (churn) presents a substantial financial risk to business sustainability. This project delivers a data-driven approach to identifying at-risk customers by analyzing demographic patterns, service usage metrics, and historical account behavior. 

Rather than treating machine learning purely as a statistical exercise, this model evaluates predictions through a strategic business lens—optimizing the model to minimize the high financial cost of missing a true churner.

## 📊 Business Logic & Model Optimization
In a real production environment, misclassifying a loyal customer as a churn risk (**False Positive**) incurs a minor cost (e.g., sending an unnecessary promotional email or retention discount). However, failing to catch a customer who is actually about to leave (**False Negative**) results in a total loss of lifetime customer value.

To reflect this economic reality, this pipeline prioritizes **Recall over Precision** during evaluation:
* **Precision Profile:** The precision score for non-churners sits at `0.43`.
* **The Strategic Trade-Off:** This deliberately lower threshold allows the model to act aggressively. We accept over-targeting stable accounts with proactive outreach in exchange for successfully capturing the vast majority of true revenue-threat risks.

## 🛠️ Technical Stack
* **Core Language:** Python
* **Data Processing & EDA:** Pandas, NumPy
* **Visualization & Documentation:** Matplotlib, Seaborn
* **Machine Learning Pipeline:** Scikit-Learn (Data Preprocessing, Column Transformers, Classification Models)

## 📂 Repository Structure
```text
├── Churn Prediction.ipynb   # Exploratory Data Analysis (EDA) & Model Pipelines
├── customer_churn.csv       # Dataset containing customer demographic and usage metrics
└── README.md                # Project documentation
