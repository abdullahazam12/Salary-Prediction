# Salary Prediction using Ensemble Learning

This project is part of the IBM PBEL AI Internship program. It focuses on predicting whether an individual earns more than $50K annually based on demographic and employment-related features. The solution uses ensemble machine learning techniques to improve accuracy and performance.

---

## 📌 Problem Statement

Given a dataset with features such as age, education, occupation, and hours worked per week, the task is to predict if a person’s income exceeds $50,000 per year. This is a binary classification problem.

---

## 📂 Dataset

The dataset is derived from the UCI Census Income dataset and contains both categorical and numerical data.

- `salary_train.csv` – Training data (11,000 rows, 12 features)
- `salary_test.csv` – Test data (4,000 rows, 11 features)

Key features:
- Age
- Workclass
- Education
- Marital Status
- Occupation
- Relationship
- Race
- Sex
- Hours-per-week
- Native country

---

## 🔧 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost, AdaBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🧠 Models Used

We trained and compared the following ensemble models:

- ✅ Random Forest Classifier
- ✅ XGBoost Classifier
- ✅ AdaBoost Classifier
- ✅ Voting Classifier (final model using soft voting)

---

## ⚙️ Data Preprocessing

- Handled missing values using median imputation
- Encoded categorical features using LabelEncoder and OneHotEncoder
- Performed feature selection using correlation and model importance
- Scaled numeric features where needed

---

## 🧪 Results

The final model (Voting Classifier) achieved:
- **Training Accuracy:** 89%  
- **Test Accuracy:** ~86%  
- Output predictions were saved in `predicted_salaries.csv`

---

## 🧩 Challenges & Solutions

| Challenge | Solution |
|----------|----------|
| High-cardinality categorical features | Used Label/OneHot Encoding appropriately |
| Overfitting risk in ensemble models | Applied cross-validation and hyperparameter tuning |
| Imbalanced data | Evaluated using precision, recall, and F1-score |

---

## 📬 Conclusion

This project demonstrates the power of ensemble learning for classification problems. Ensemble models improved the accuracy and stability of predictions. Future improvements could include deeper hyperparameter tuning and trying stacked generalization.

---

## 🙌 Acknowledgements

- IBM SkillsBuild & PBEL AI Internship Team
- UCI Machine Learning Repository
- Scikit-learn, XGBoost, and open-source contributors