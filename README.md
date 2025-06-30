# Logistic-Regression-Classifier-with-GridSearch-Imbalanced-Data-Handling


**# 🩺 CHD Risk Prediction - Logistic Regression Model**

This project uses a real-world dataset from the **Framingham Heart Study** to build a binary classification model that predicts whether a person is at risk of developing **Coronary Heart Disease (CHD)** within the next 10 years.

---

**## 📊 Dataset Overview**

The dataset consists of **4,238 patient records** with demographic, behavioral, and medical risk factors. It is commonly used for predicting heart disease risk using supervised machine learning.

### 🎯 Target Variable
- `TenYearCHD`: 
  - `1` → Patient developed CHD in the next 10 years
  - `0` → Patient did not develop CHD

**### 📥 Feature Variables**

| Feature             | Description                                        |
|---------------------|----------------------------------------------------|
| `male`              | 1 = male, 0 = female                               |
| `age`               | Age in years                                       |
| `education`         | Education level (1 to 4)                           |
| `currentSmoker`     | Whether the person currently smokes               |
| `cigsPerDay`        | Cigarettes smoked per day                         |
| `BPMeds`            | On blood pressure medication                      |
| `prevalentStroke`   | History of stroke (1 = yes)                       |
| `prevalentHyp`      | History of hypertension                           |
| `diabetes`          | Has diabetes (1 = yes)                            |
| `totChol`           | Total cholesterol                                 |
| `sysBP`             | Systolic blood pressure                           |
| `diaBP`             | Diastolic blood pressure                          |
| `BMI`               | Body Mass Index                                   |
| `heartRate`         | Heart rate (beats per minute)                     |
| `glucose`           | Glucose level                                     |

---

**## 🧠 Project Objectives**

- Clean and preprocess the dataset
- Handle missing values
- Build a **Logistic Regression** model
- Use **GridSearchCV** to tune hyperparameters
- Apply **class balancing techniques** to handle imbalanced data
- Evaluate model using classification metrics like accuracy, recall, F1-score, and ROC-AUC

---

**## 🛠️ Tech Stack**

- **Python**
- **Pandas & NumPy** for data manipulation
- **Scikit-learn** for modeling, preprocessing, and evaluation

---

**## 📈 Model Performance**

| Metric        | Value     |
|---------------|-----------|
| Accuracy      | 68.5%     |
| Recall (CHD=1)| 68%       |
| F1-Score (CHD=1) | 0.41   |

> While accuracy dropped from 85% to 68.5%, the recall for the minority class improved significantly — from **6% to 68%**, making the model much more reliable for medical screening.

---
**🔍 Future Improvements**


Add ROC curves and confusion matrix visualizations


Try advanced models (RandomForest, XGBoost, LightGBM)


Explore threshold tuning for higher precision


Deploy model with Flask or Streamlit


## 📂 How to Use
*1. Clone this repo:*
git clone https://github.com/rohan-sharma82/chd-risk-logistic-model.git
cd chd-risk-logistic-model


*2 Install dependencies:*

bash-
pip install -r requirements.txt
Run the notebook or script:

bash-
python chd_model.py
