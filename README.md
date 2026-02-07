# Titanic Survival Analysis – EDA & Preprocessing

## Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** and **data preprocessing** on the famous **Titanic dataset** to identify key factors influencing passenger survival. The analysis was completed as **Task 2** during my internship at **Elevvo Pathways**.

---

## Objectives

* Understand the structure and quality of the dataset
* Analyze survival patterns based on key features
* Handle missing values and outliers
* Engineer meaningful features
* Prepare the data for machine learning models

---

##  Dataset Information

* Total records: **891**
* Target variable: **Survived** (0 = No, 1 = Yes)
* Key features analyzed:

  * Sex
  * Pclass
  * Age
  * Fare
  * SibSp
  * Parch

---

##  Exploratory Data Analysis (EDA)

The EDA phase focused on understanding feature distributions and their relationship with survival:

* Survival rate comparison by **gender**
* Survival patterns across **passenger classes**
* Distribution analysis for **Age** and **Fare**
* Impact of **family size** on survival probability

Visualizations were created using **Matplotlib** and **Seaborn**.

---

##  Data Cleaning & Preprocessing

* Missing values handled:

  * Age: imputed using **mean**
  * Embarked: imputed using **mode**
* Removed irrelevant features:

  * PassengerId, Name, Ticket, Cabin
* Outliers in **Age** and **Fare** were treated using percentile-based clipping

---

## Feature Engineering

* Categorical encoding:

  * One-Hot Encoding for **Sex** and **Embarked**
* New features created:

  * **FamilySize** = SibSp + Parch + 1
  * **IsAlone** (binary indicator)
* Feature scaling applied using **StandardScaler**

---

##  Modeling

* Algorithm used: **Logistic Regression**
* Train-test split applied
* Model evaluated using accuracy metric

### Result

* Test Accuracy: **76.92%**

---

## Key Insights

* Females had a significantly higher survival rate than males
* First-class passengers were more likely to survive
* Passengers with small family sizes showed better survival chances

---

## Tools & Libraries

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

---

##  Project Structure

```
Titanic_preprocessing.ipynb
README.md
```

---

⭐ If you found this project useful, feel free to give it a star!
