# 🎯 Sonar Rock vs. Mine Prediction: Classification of Sonar Signals

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.5-orange)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made in Egypt](https://img.shields.io/badge/Made%20in-Egypt-red)](https://en.wikipedia.org/wiki/Egypt)

---

## 📖 Project Description

This is a **classic and popular Machine Learning project** in the field of Data Science.

Its goal is to **distinguish** between sonar signals returned from an underwater **Rock** or a **Metallic Mine** using 60 numerical features extracted from sonar frequencies.

> The Famous Dataset: [UCI Sonar Dataset](https://archive.ics.uci.edu/dataset/151/connectionist+bench+sonar+mines+vs+rocks)

---

## 🚀 Results Achieved (So Far)

| Model | Accuracy | Notes |
| :--- | :--- | :--- |
| Logistic Regression | ~ 78-82% | Quick baseline model |
| Random Forest (Untuned) | ~ 85-90% | Strong performance out of the box |
| **Random Forest + Tuning** | **~ 90-94%** | Best model after using `RandomizedSearchCV` |

---

## 🛠 Tools and Libraries Used

* **Python**
* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn`
* **Visualization:** `matplotlib` & `seaborn`
* **Environment:** Jupyter Notebook

---

---

## ⚙️ Key Techniques and Solutions Applied

* Used **`StandardScaler`** to improve Logistic Regression performance.
* Split the data using **`stratify=y`** to ensure an equal distribution of both classes.
* Solved the issue with string labels when using `scoring='f1'` by switching to **`f1_macro`**.
* Tuned the **Random Forest** model using **`RandomizedSearchCV`** (40 iterations).
* Comprehensive evaluation: Accuracy, **Classification Report**, and **Confusion Matrix**.

---

## 🎯 Proposed Future Enhancements

* [ ] Experiment with **SVM with RBF kernel** (often reaches 96–98% accuracy).
* [ ] Apply **PCA (Principal Component Analysis)** for dimensionality reduction.
* [ ] Use **`GridSearchCV`** or **Optuna** for more granular hyperparameter tuning.
* [ ] Save the best model using **`joblib`** and load it for fast prediction.
* [ ] Convert the project into a **Streamlit Web App**.
* [ ] Create a **Docker container** for portability.

---

## 🚀 How to Run the Project

```bash
git clone [https://github.com/MuhammadSeyam/Sonar-prediction-Rock-vs-Mine.git](https://github.com/MuhammadSeyam/Sonar-prediction-Rock-vs-Mine.git)
cd Sonar-prediction-Rock-vs-Mine
jupyter notebook Sonar.ipynb
