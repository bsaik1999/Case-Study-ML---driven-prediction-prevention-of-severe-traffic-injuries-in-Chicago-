# 🚦 Chicago Traffic Crash Severity Prediction
🔍 A data-driven machine learning pipeline for analyzing traffic crash records in Chicago (2016–2024) to identify key factors leading to severe injuries.

---

## 🚀 What It Does
- Preprocesses **Chicago Police Department traffic crash reports**  
- Embeds categorical crash attributes with one-hot encoding & dimensionality reduction  
- Performs exploratory data analysis:
  - Class imbalance analysis  
  - Missing data visualization  
  - Chi-squared association tests (Cramér’s V)  
- Trains and evaluates multiple classifiers:
  - Logistic Regression (baseline & LASSO regularized)  
  - LDA / QDA  
  - CART, Random Forest, Bagging, Gradient Boosting  
- Optimizes thresholds using **Youden’s J statistic**  
- Provides interpretability via:
  - Odds ratios (LASSO)  
  - SHAP values (GBM)  
  - Partial Dependence Plots (Speed Limit impact)  
  - Multiple Correspondence Analysis (MCA)

---

## 📊 Key Findings
- Severe injuries occur in **~18.6% of crashes** (class imbalance challenge).  
- **Pedestrian crashes, driver physical condition, and high speed limits** strongly drive severity.  
- **GBM and LASSO regression** achieved the highest predictive performance (AUC ≈ 0.60).  
- MCA and SHAP highlight **trafficway type, contributory causes, and crash type** as dominant features.  

---

## 🧠 Core Tech Stack
- **R (tidyverse, caret, glmnet, pROC, FactoMineR, factoextra)**  
- **Statistical modeling:** Logistic regression, LDA, QDA  
- **Machine learning:** Random Forest, Gradient Boosting, LASSO  
- **Interpretability:** SHAP (fastshap), PDP (pdp), MCA  

---

