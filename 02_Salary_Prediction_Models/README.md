# 💰 Salary Prediction Models: Regression Algorithms Comparison

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 🎯 Project Overview
This project focuses on evaluating and comparing various regression algorithms using a dataset of employee salaries based on their title levels. The main goal is to understand how different machine learning models perform on the exact same dataset and which one provides the most accurate salary predictions.

## 🧠 Machine Learning Models Implemented
To find the best fit, I have applied and compared the following regression algorithms:
1. **Linear Regression**
2. **Polynomial Regression**
3. **Support Vector Regression (SVR)** *(with feature scaling)*
4. **Decision Tree Regression**
5. **Random Forest Regression**

## 🛠️ Data Preprocessing & Engineering
- **Feature Selection:** Evaluated the impact of different columns on the target variable using P-values. Eliminated highly irrelevant variables and kept only the `Title Level` (Unvan Seviyesi) to avoid confusing the models.
- **Scaling Strategies:** Applied `StandardScaler` specifically for the SVR model, as distance-based algorithms require scaled data for optimal performance. Conversely, tree-based algorithms (Decision Tree & Random Forest) were fed with the original unscaled data, demonstrating an understanding of each algorithm's underlying mathematical requirements.

## 📂 Project Structure
```text
├── maaslar_yeni.csv         # Salary dataset
├── proje.ipynb              # Jupyter Notebook containing all algorithms & R² evaluations
└── README.md                # Project documentation
```

📊 Results & Model Evaluation
Model performances were strictly evaluated using the R-squared (R²) metric via r2_score. The results clearly demonstrated that non-linear and tree-based algorithms (especially Random Forest and higher-degree Polynomial Regression) significantly outperformed the standard linear approach for this specific dataset.

💻 Installation & Usage
1. Clone the repository

```Bash

git clone [https://github.com/Vooguz/AI-Projects-Portfolio.git](https://github.com/Vooguz/AI-Projects-Portfolio.git)
cd AI-Projects-Portfolio/02_Salary_Prediction_Models
```
2. Run the Notebook
Open proje.ipynb to see the step-by-step implementation, visual plots, and the final R² score comparisons.

👨‍💻 Author
Oğuz Eren

Computer Engineering Student @ Uludağ University

GitHub: @Vooguz
