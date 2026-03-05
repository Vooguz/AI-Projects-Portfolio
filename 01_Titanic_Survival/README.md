# 🚢 Titanic Survival Prediction (My First ML Project)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?style=for-the-badge&logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 🎯 Project Overview
This project marks one of my first steps into the world of Machine Learning. Working with the legendary Titanic dataset, I focused on developing fundamental data science skills, including data cleaning, missing value imputation, categorical data encoding, and feature scaling.

## 🧠 Learning Process & Model Selection (Author's Note)
*When I developed this project, I hadn't yet been introduced to Classification algorithms. Therefore, even though this is fundamentally a classification problem (Survived: 1 / Did Not Survive: 0), I utilized the tools I had at the time and implemented a **Multiple Linear Regression** model.*

*I built my own classification logic by using the `round()` function as a "hack" to convert the continuous decimal outputs of the regression model into discrete 0s and 1s. While `Logistic Regression` is the industry standard for this task, I kept this original approach in the repository as it reflects my problem-solving skills and my early learning methodology.*

## 🛠️ Technical Architecture & Preprocessing
The strongest aspect of this project is the data preparation pipeline before feeding it into the model:
1. **Handling Missing Data:** Missing values in the `Age` and `Fare` columns were imputed using the mean strategy via `SimpleImputer`.
2. **Categorical Encoding:** The `Sex` variable was converted using `LabelEncoder`, and the `Embarked` variable was transformed into a machine-readable format using `OneHotEncoder`.
3. **Feature Scaling:** The dataset was standardized using `StandardScaler` to ensure model stability.
4. **Backward Elimination:** P-values were calculated using the `statsmodels` library to identify and remove statistically insignificant features from the dataset.

## 📂 Project Structure
```text
├── train.csv                # Training dataset
├── test.csv                 # Testing dataset
├── gender_submission.csv    # Sample submission format
├── titanic.ipynb            # Jupyter Notebook with full analysis & code
└── README.md                # Project documentation
```
📊 Model Performance
Using my custom Regression + Rounding logic, the model achieved an accuracy of 78.9% on the test dataset.

💻 Installation & Usage
1. Clone the repository

```Bash

git clone [https://github.com/Vooguz/AI-Projects-Portfolio.git](https://github.com/Vooguz/AI-Projects-Portfolio.git)
cd AI-Projects-Portfolio/01_Titanic_Survival
```
2. Run the Notebook
Open titanic.ipynb in Jupyter Notebook, JupyterLab, or VS Code to view the exploratory data analysis, preprocessing steps, and model training.

👨‍💻 Author
Oğuz Eren
Computer Engineering Student @ Uludağ University
GitHub: @Vooguz
