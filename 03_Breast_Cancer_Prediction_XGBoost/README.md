# 🧬 Breast Cancer Diagnosis with XGBoost & Ablation Study

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-Machine%20Learning-ebbc00?style=for-the-badge)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Analysis-orange?style=for-the-badge&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 🎯 Project Overview
This project focuses on predicting breast cancer diagnosis (Malignant vs. Benign) using the **WDBC (Wisconsin Diagnostic Breast Cancer)** dataset. Beyond simple classification, this study dives deep into **Feature Engineering** and **Model Robustness** through advanced selection techniques and an Ablation Study.

## 🧠 Technical Highlights
- **XGBoost Classifier:** Utilized high-performance gradient boosting for maximum accuracy.
- **Advanced Feature Selection:**
    - **Variance Threshold:** Identifying low-variance features.
    - **Correlation Analysis:** Removing redundant features (threshold > 0.9) to reduce noise.
    - **Feature Importance:** Using XGBoost's gain metrics to filter the most impactful variables.
- **Ablation Study:** A systematic evaluation where the top 5 most important features were removed one by one to test the model's dependency and stability.

## 📊 Key Results
- **Baseline Accuracy:** ~97.37%
- **Baseline F1-Score:** ~0.9639
- **Ablation Insight:** Removing the most critical feature (`concave_points_mean`) led to the most significant drop in performance, proving its diagnostic value.

## 📂 Project Structure
```text
├── wdbc.data                # Raw dataset (WDBC)
├── proje.ipynb              # Full pipeline: EDA, Feature Engineering, XGBoost, Ablation Study
└── README.md                # Project documentation
```

💻 Installation & Usage
1. Clone the repository

```Bash

git clone [https://github.com/Vooguz/AI-Projects-Portfolio.git](https://github.com/Vooguz/AI-Projects-Portfolio.git)
cd AI-Projects-Portfolio/03_Breast_Cancer_Prediction_XGBoost
```
2. Install dependencies
```Bash

pip install xgboost pandas numpy seaborn matplotlib scikit-learn
```

3. Run the analysis
Execute the proje.ipynb notebook to see the full diagnostic workflow and visualization of results.

👨‍💻 Author
Oğuz Eren

Computer Engineering Student @ Uludağ University

GitHub: @Vooguz
