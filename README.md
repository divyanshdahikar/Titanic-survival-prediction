# 🚢 Titanic Survival Prediction

This project uses Machine Learning to predict whether a passenger survived the Titanic disaster based on various features like age, gender, class, and fare. It includes thorough data cleaning, visualization, and model building using classification algorithms.

---

## 🧠 Project Objective

To predict passenger survival on the Titanic using classification models by analyzing patterns in the dataset and applying data preprocessing and feature engineering techniques.

---

## 📁 Dataset

Used the [Kaggle Titanic dataset](https://www.kaggle.com/competitions/titanic/data) which contains:

* `PassengerId`, `Name`, `Sex`, `Age`, `Pclass`
* `SibSp`, `Parch`, `Fare`, `Cabin`, `Embarked`
* `Survived` (Target variable)

### Data Cleaning Highlights:

* Handled missing values (`Age`, `Embarked`, `Cabin`)
* Converted categorical variables (`Sex`, `Embarked`) to numeric
* Dropped irrelevant columns (`Name`, `Ticket`, `Cabin`)
* Created new features (e.g., `FamilySize`, `IsAlone`)

---

## 🧹 Data Preprocessing

* Used `LabelEncoder` and `OneHotEncoding` for categorical variables
* Filled missing `Age` values using median imputation
* Scaled numerical features for better model performance

---

## 📊 Exploratory Data Analysis

Visualized insights like:

* Survival rate by gender and passenger class
* Distribution of age, fare, and family size
* Correlation heatmap of key features
* Count plots for survival vs class, gender, embark location
![Screenshot 2025-06-18 141925](https://github.com/user-attachments/assets/93a17fb0-a2ef-487e-9da0-6287980a97d7)

---

## 🤖 Model Building

### Features:

* `Pclass`, `Sex`, `Age`, `Fare`, `Embarked`, `FamilySize`, `IsAlone`

### Classifier:

* **Logistic Regression**

### Performance:

* **Accuracy: 83.22580645161291%** on test data (Logistic Regression)

---

## 🔍 Sample Predictions

| Passenger Class | Gender | Age | Fare  | Predicted Survival |
| --------------- | ------ | --- | ----- | ------------------ |
| 1               | Male   | 45  | 80.00 | Survived           |
| 3               | Female | 21  | 7.25  | Survived           |
| 2               | Male   | 33  | 13.00 | Not Survived       |

---

## 📦 Tech Stack

* Python 🐍
* Pandas & NumPy
* Scikit-learn
* Seaborn & Matplotlib
* Jupyter Notebook

---

## 📌 How to Run

1. Clone the repository
2. Install dependencies

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Open the notebook

   ```bash
   jupyter notebook Titanic_Survival_Prediction.ipynb
   ```
