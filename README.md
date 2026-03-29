# 🧠 Customer Churn Prediction using ANN (Deep Learning Project)

## 📌 Overview

This project focuses on predicting **customer churn** using an Artificial Neural Network (ANN).

Customer churn refers to customers leaving a service or business. By analyzing customer data such as demographics, account details, and financial behavior, this model predicts whether a customer is likely to exit or stay.

The project demonstrates how **deep learning techniques** can be applied to solve real-world business problems like customer retention and revenue optimization.

---

## 🎯 Objective

The main objective of this project is to build a predictive model that identifies customers who are likely to churn.

It aims to:

* Analyze customer behavior and patterns
* Perform data preprocessing and feature engineering
* Build and train an Artificial Neural Network (ANN)
* Evaluate model performance using accuracy and confusion matrix
* Help businesses take proactive actions to reduce churn

---

## 📂 Dataset Description

The dataset contains the following features:

* **RowNumber** – Row index
* **CustomerId** – Unique customer ID
* **Surname** – Customer surname
* **CreditScore** – Credit score of the customer
* **Geography** – Country of the customer
* **Gender** – Male/Female
* **Age** – Age of the customer
* **Tenure** – Number of years with the bank
* **Balance** – Account balance
* **NumOfProducts** – Number of products used
* **HasCrCard** – Credit card status (1 = Yes, 0 = No)
* **IsActiveMember** – Active membership status
* **EstimatedSalary** – Estimated salary
* **Exited** – Target variable (1 = Churn, 0 = Stay)

---

## 🛠️ Technologies Used

* Python 🐍
* TensorFlow / Keras 🤖
* NumPy & Pandas
* Matplotlib 📊
* Scikit-learn

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing

* Loaded dataset using Pandas
* Selected relevant features
* Converted categorical variables using **One-Hot Encoding**
* Split dataset into training and testing sets
* Applied **feature scaling** using StandardScaler

---

### 2️⃣ Model Building (ANN)

* Built ANN using **Keras Sequential API**
* Architecture:

  * Input Layer
  * Hidden Layer (11 neurons, ReLU)
  * Hidden Layer (6 neurons, ReLU)
  * Output Layer (1 neuron)

---

### 3️⃣ Model Compilation

```python
classifier.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
```

---

### 4️⃣ Model Training

* Trained model with:

  * Epochs: 50
  * Batch size: 10
  * Validation split: 0.33

---

### 5️⃣ Model Evaluation

* Generated predictions on test data
* Used **Confusion Matrix** to evaluate performance
* Calculated model accuracy

```python
Accuracy ≈ 85.8%
```

---

## 📊 Results & Insights

* The ANN model achieved **~85% accuracy**, indicating good predictive performance
* The model successfully distinguishes between churned and retained customers
* Features like **age, balance, and activity status** play a significant role in churn prediction

---

## 📈 Visualization

* Training vs Validation Accuracy plotted using Matplotlib
* Helps in understanding model performance and overfitting

---

## 🧠 Key Learnings

* Data preprocessing is crucial for machine learning models
* Feature scaling improves ANN performance
* Neural networks can effectively model complex patterns
* Evaluation metrics like confusion matrix provide deeper insights

---

## 🚀 Conclusion

This project demonstrates how deep learning can be used to predict customer churn and support business decision-making.

By identifying customers at risk of leaving, companies can take targeted actions to improve retention and increase profitability.

---

## ⭐ Future Improvements

* Hyperparameter tuning
* Use of Dropout layers to reduce overfitting
* Try advanced models (Random Forest, XGBoost)
* Deploy model using Streamlit or Flask

---

⭐ *Feel free to fork, star ⭐, and contribute!*
