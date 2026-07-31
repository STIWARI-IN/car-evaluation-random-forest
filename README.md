# 🚗 Car Evaluation Classification Using Random Forest

A machine learning project that predicts the acceptability of cars using the **Random Forest Classifier**. The project includes data preprocessing, categorical feature encoding, model training, hyperparameter tuning with **GridSearchCV**, and model evaluation using multiple classification metrics.

## 📌 Project Overview

The objective of this project is to classify cars into one of the following categories:

* **unacc** – Unacceptable
* **acc** – Acceptable
* **good** – Good
* **vgood** – Very Good

The model is trained on the **Car Evaluation Dataset** using the Random Forest algorithm and optimized through hyperparameter tuning.

---

## 📂 Dataset

The dataset contains the following features:

| Feature  | Description                         |
| -------- | ----------------------------------- |
| buying   | Buying price                        |
| maint    | Maintenance cost                    |
| doors    | Number of doors                     |
| persons  | Passenger capacity                  |
| lug_boot | Luggage boot size                   |
| safety   | Safety rating                       |
| class    | Target variable (Car Acceptability) |

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📋 Project Workflow

1. Load the dataset
2. Explore the data
3. Preprocess categorical features
4. Encode categorical variables
5. Split the dataset into training and testing sets
6. Train a Random Forest Classifier
7. Tune hyperparameters using GridSearchCV
8. Evaluate the model using:

   * Confusion Matrix
   * Classification Report
   * Accuracy Score
   * Precision
   * Recall
   * F1-Score

---

## 📊 Model Performance

| Metric            |    Score |
| ----------------- | -------: |
| Accuracy          |  **93%** |
| Macro F1-Score    | **0.83** |
| Weighted F1-Score | **0.94** |

### Classification Report

| Class | Precision | Recall | F1-Score |
| ----- | --------: | -----: | -------: |
| acc   |      0.89 |   0.83 |     0.86 |
| good  |      0.57 |   0.84 |     0.68 |
| unacc |      1.00 |   0.97 |     0.98 |
| vgood |      0.69 |   1.00 |     0.81 |

### Summary

* Achieved **93% overall accuracy**.
* Excellent performance on the **unacc** class (F1-score: **0.98**).
* Strong performance on **acc** and **vgood** classes.
* Significantly improved detection of the minority **good** class after hyperparameter tuning.
* The **macro F1-score of 0.83** indicates balanced performance across all classes despite class imbalance.

---

## 📈 Future Improvements

* Compare Random Forest with XGBoost, LightGBM, and CatBoost.
* Perform feature importance analysis.
* Deploy the trained model as a web application using Streamlit or Flask.
* Experiment with additional hyperparameter optimization techniques.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Sudhir Tiwari**

If you found this project helpful, consider giving the repository a ⭐ on GitHub.
