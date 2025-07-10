
# 📊 Bank Marketing Term Deposit Prediction

This project analyzes customer data from a Brazilian bank to predict whether a client will subscribe to a term deposit. The analysis includes EDA, preprocessing, baseline modeling, class imbalance handling.
# 📊 Bank Marketing Term Deposit Prediction

[🔗 View this project on GitHub](https://github.com/SatyamWadhwa882/bank-eda.git)

This project analyzes customer data from a Brazilian bank...



## 📁 Dataset Summary

- Customers contacted by phone for term deposit subscription.
- Target variable: `TARGET` (yes/no)
- Features include age, job, marital status, education, balance, loan status, contact details, etc.

## 🔍 Exploratory Data Analysis (EDA)

- Class imbalance observed (`~88%` no, `~12%` yes)
- Job types like *student* and *retired* show higher conversion rates
- Longer call duration correlates positively with subscription

## 🛠️ Preprocessing

- Handled `"unknown"` as missing values (kept as is for modeling)
- Categorical variables encoded via `get_dummies()`
- Train-test split with stratification on `TARGET`
- SMOTE applied to handle class imbalance

## 🤖 Model & Metrics

**Baseline Model**: Random Forest  
- Accuracy: 0.85  
- F1 Score: 0.49  
- AUC: 0.92

**After SMOTE**:  
- F1 Score: 0.53  
- AUC: 0.92  

## 📈 Visual Insights

- Bar plots, boxplots, stacked bar %, and FacetGrid visualizations used
- Strong visual correlation between marital status, education, and subscription

## 📌 Files Included

- `Step_5_Brief_Evaluation_Summary.docx`: Final written analysis
- `Bank_Marketing_Original_Data.csv`: Dataset
- Python scripts / notebooks (optional)

## 🚀 Next Steps

- Hyperparameter tuning with `GridSearchCV`
- Feature engineering on `balance`, `age`
- Model threshold optimization
- Integration into an end-to-end app or dashboard

---

Made with ❤️ for ML interpretability and reproducible analysis.
