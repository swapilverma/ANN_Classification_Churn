## ANN_Classification_Churn

# 🧠 ANN Classification - Customer Churn Prediction  

This repository contains an **Artificial Neural Network (ANN)** model designed to predict whether a customer is likely to churn based on various features. The dataset includes customers from **France, Germany, and Spain**, and categorical variables are encoded before training the model.  

Additionally, a **Streamlit app (`app.py`)** is included to visualize customer churn predictions interactively.  


---

## 📂 Project Overview  

- **Objective:** Predict if a customer will churn using an ANN model.  
- **Data Preprocessing:**  
  - **Gender** - Encoded using **Label Encoding**.  
  - **Geography (France, Germany, Spain)** - Encoded using **One-Hot Encoding**.  

---

## 🏗️ ANN Model Architecture  

A **Sequential ANN model** was implemented with the following layers:  

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

model = Sequential([
    Dense(64, activation='relu', input_shape=(X_train.shape[1],)),  # HL1 Connected with Input Layer
    Dense(32, activation='relu'),  # HL2
    Dense(1, activation='sigmoid')  # Output Layer
])
```

## 🛠️ Tools and Libraries Used
#### 📌 Programming Language
 - Python
#### 📌 Libraries
- TensorFlow & Keras - Model building
- Pandas - Data manipulation
- NumPy - Numerical computations
- Scikit-learn - Data preprocessing
- Matplotlib & Seaborn - Data visualization
- Streamlit - Web-based visualization

## 📈 Model Performance
- **Training Accuracy:** 87.25%
- **Validation Accuracy:** 85.35%

## Streamlit Interface 
![image](https://github.com/user-attachments/assets/620f52d3-69d9-4cdb-bae9-780d8a75572d)


## 🚀 How to Use

git clone https://github.com/swapilverma/ANN_Classification_Churn.git





