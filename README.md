### Flipkart_Customer_Classification_ML_capstone_project

<img width="251" height="178" alt="image" src="https://github.com/user-attachments/assets/a7b1b255-bb4d-4466-b075-fac6e3cc4bc3" />



* **Project Title:** Flipkart Customer Service Satisfaction Analysis
* **Goal:** Predict customer satisfaction (CSAT) and identify improvement areas.
* **Tech Stack:** Python, Pandas, Matplotlib, Scikit-learn, SMOTE,etc.
* **Key Steps:** EDA, Data Preprocessing, Feature Engineering, Modeling, Evaluation,etc 
* **Results Summary:**  The classification models were evaluated based on Accuracy, Precision, Recall, and F1-Score.
After multiple experiments, XGBoost emerged as the best-performing model.

--> *Best Model:* XGBoost Classifier

--> *Accuracy:* ~90%

--> *Precision:* 0.89

--> *Recall:* 0.87

--> *F1-Score:* 0.88

XGBoost outperformed Logistic Regression and Random Forest due to its ability to handle class imbalance and capture non-linear feature relationships.
This model effectively distinguishes between satisfied and dissatisfied customers, enabling Flipkart to focus on customers who are more likely to churn.

XGBoost achieved the highest accuracy of around 90%, outperforming Logistic Regression and Random Forest models.
The model effectively classified customers as Satisfied or Not Satisfied, even with class imbalance handled using SMOTE.
Key insights revealed that faster response times, quick resolutions, and experienced agents were major contributors to higher customer satisfaction.



## 📘 Project Overview
This project focuses on predicting **Customer Satisfaction (CSAT)** for Flipkart’s customer service interactions.  
The goal is to transform raw support data into actionable insights to improve service quality and customer experience.

---

## 🎯 Problem Statement
Customer satisfaction is crucial for retaining users and maintaining brand reputation.  
Flipkart aims to understand which factors (like response time, issue type, and agent performance) most impact satisfaction scores.

---

## 🧠 Objectives
- Analyze customer service data to identify key satisfaction drivers.  
- Build a classification model to predict customer satisfaction (High/Low CSAT).  
- Suggest actionable insights to enhance service performance.

---

## 🧩 Dataset Overview
- **Total Records:** 85,907  
- **Total Columns:** 20  
- **Target Variable:** `CSAT Score` (transformed into binary: High / Low)  
- **Key Features:** Channel, Category, Response Time, Resolution Days, Agent Shift, and Tenure Bucket.

---

## 🔍 Exploratory Data Analysis (EDA)
- Found **no duplicate rows**.
- **Missing values** in certain columns (e.g., `Customer City`, `Item_price`, `Customer Remarks`).
- CSAT scores of **4 and 5** dominate, indicating high overall satisfaction.
- Response time and resolution days play a major role in satisfaction.

---

## 🧮 Feature Engineering
- Created new features:
  - `response_time_mins`  
  - `resolution_days`  
  - `issue_day_of_week`, `issue_hour`, `is_weekend`  
  - `time_of_day` (Morning, Afternoon, Evening, Night)
- Handled class imbalance using **SMOTE**.
- Encoded categorical variables for ML compatibility.

---

## ⚙️ Machine Learning Models
| Model | Accuracy | Comments |
|--------|-----------|----------|
| Logistic Regression | ~82% | Good baseline performance |
| Random Forest | ~88% | Balanced performance & interpretability |
| XGBoost | ~90% | Best accuracy and robustness |

---

## 📊 Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score used for performance evaluation.  
- Addressed **class imbalance** to improve minority class prediction.  
- Analyzed **feature importance** to identify top drivers of satisfaction.

---

## 💡 Key Insights
- **Returns** and **Order-Related** issues dominate support cases.  
- **Faster response times** correlate strongly with higher CSAT.  
- **Agent tenure** and **shift timing** affect customer experience.  
- Email and Outcall channels need service improvement.

---

## 🚀 Business Impact
- Helps Flipkart identify areas to **reduce churn** and **improve loyalty**.  
- Provides data-driven strategies for **training**, **channel optimization**, and **workflow improvement**.

---

## 🧩 Future Work
- Incorporate **textual data** (customer remarks) using **NLP techniques**.  
- Experiment with **deep learning models** for sentiment-based prediction.  
- Further optimize model for minority (Low CSAT) class prediction.

---

## 🧠 Technologies Used
- Python, Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn, XGBoost, imbalanced-learn (SMOTE)  
- Google Colab, GitHub

---

## 🏁 Conclusion
This project demonstrates how structured customer service data can be leveraged to predict satisfaction and guide strategic improvements in customer experience, leading to stronger retention and brand growth.
