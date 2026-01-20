
---

# 💻 Laptop Price Prediction System

*A Machine Learning Web Application using Streamlit*

---

## 📌 Project Overview

The **Laptop Price Prediction System** is an end-to-end **machine learning web application** that predicts the **price of a laptop** based on its specifications such as brand, RAM, CPU, GPU, storage, screen size, resolution, and other hardware features.

This project demonstrates the **complete ML lifecycle**:

* Data preprocessing
* Feature engineering
* Model training & pipeline creation
* Model serialization
* Web app deployment using **Streamlit**

The application provides a **user-friendly interface** where users can input laptop specifications and instantly receive a **predicted market price**.

---

## 🎯 Problem Statement

Laptop prices vary significantly depending on multiple hardware and software factors. Manually estimating a fair price is difficult for customers, sellers, and analysts.

This project solves that problem by:

* Learning patterns from historical laptop data
* Predicting prices using machine learning
* Providing real-time predictions through a web app

---

## 🧠 Machine Learning Approach

* Dataset contains real laptop specifications and prices
* Categorical and numerical features are processed together
* A **pipeline** is used to ensure consistent preprocessing and prediction
* The target variable (price) is **log-transformed** for better model performance
* Final predictions are converted back using exponential transformation

---

## 🛠 Tech Stack

### 🔹 Programming & Libraries

* Python
* NumPy
* Pandas
* Scikit-learn

### 🔹 Web Framework

* Streamlit

### 🔹 Model & Storage

* Machine Learning Pipeline (`pipe.pkl`)
* Processed DataFrame (`df.pkl`)

### 🔹 Deployment Support

* `requirements.txt`
* `Procfile`
* `setup.sh`

---

## 📂 Project Structure

```
Laptop-Price-Prediction
│
├── app.py                         # Streamlit web application
├── Laptop_Price_Prediction.ipynb  # Model training & analysis
├── laptop_data.csv                # Dataset
├── pipe.pkl                       # Trained ML pipeline
├── df.pkl                         # Processed dataframe
├── requirements.txt               # Dependencies
├── Procfile                       # Deployment config
├── setup.sh                       # Streamlit server setup
└── README.md
```

---

## 🖥️ Web App Features

The Streamlit application allows users to input:

* Brand (Company)
* Laptop Type
* RAM size
* Weight
* Touchscreen support
* IPS Display
* Screen Size
* Screen Resolution
* CPU Brand
* HDD Storage
* SSD Storage
* GPU Brand
* Operating System

### 🔍 Feature Engineering

* **PPI (Pixels Per Inch)** is calculated dynamically using screen size and resolution
* Binary features are created for touchscreen and IPS display

---

## ⚙️ How Prediction Works

1. User enters laptop specifications
2. Inputs are transformed into model-ready format
3. The trained pipeline predicts **log(price)**
4. Exponential transformation is applied
5. Final laptop price is displayed in **INR (₹)**

```python
np.exp(pipe.predict(query)[0])
```

---

## ▶️ How to Run the Project Locally

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Run Streamlit App

```bash
streamlit run app.py
```

### 3️⃣ Open in Browser

```
http://localhost:8501
```

---

## 🎓 Skills Demonstrated

* Machine Learning modeling
* Feature engineering
* Pipeline creation
* Data preprocessing
* Streamlit UI development
* ML model deployment
* End-to-end project design

---

## 📌 Use Cases

* Laptop price estimation
* E-commerce price analysis
* Data science portfolio project
* Academic / college project
* ML deployment practice

---

## 🚀 Future Enhancements

* Add brand-wise price visualization
* Support for more hardware features
* Cloud deployment (AWS / Azure)
* Mobile-friendly UI
* Model comparison & accuracy display
  
## 📸 Screenshots

### 🔹 Laptop Price Predictor – Main Interface
(<img width="1536" height="1024" alt="ChatGPT Image Jan 20, 2026, 05_50_54 PM" src="https://github.com/user-attachments/assets/68ffae74-46d4-431e-ba6c-51269414c2be" />
)

### 🔹 Input Specifications Section
(![Uploading ChatGPT Image Jan 20, 2026, 05_50_54 PM.png…]()
)

### 🔹 Price Prediction Result
![Prediction Result](screenshots/screenshot-3.png)

---

## 🏁 Conclusion

This project demonstrates how **machine learning models can be transformed into real-world applications**. By combining **data science, ML pipelines, and Streamlit**, the Laptop Price Predictor delivers accurate predictions through an intuitive interface, making it a strong **portfolio project for Data Science, ML, and Software roles**.

---


