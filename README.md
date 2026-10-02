# 🛒 Big Mart Sales Prediction

## 📌 Project Overview

**Big Mart Sales Prediction** is a Machine Learning project that predicts the sales of products across different Big Mart retail outlets using historical sales data.

The project analyzes product characteristics, outlet information, pricing, visibility, and other relevant features to identify factors influencing sales and predict **Item Outlet Sales**.

The trained model is integrated with a **Flask web application**, allowing users to provide product and outlet details and obtain a predicted sales value.

## 🎯 Objective

The main objective of this project is to develop a regression-based machine learning model capable of predicting product sales based on:

* Product characteristics
* Product visibility
* Item MRP
* Outlet characteristics
* Outlet location
* Outlet type
* Outlet establishment information

## 📊 Dataset

The dataset contains **8,523 records** and includes the following features:

* Item Identifier
* Item Weight
* Item Fat Content
* Item Visibility
* Item Type
* Item MRP
* Outlet Identifier
* Outlet Establishment Year
* Outlet Size
* Outlet Location Type
* Outlet Type
* Item Outlet Sales

## 🔍 Project Workflow

### 1. Data Loading

The historical Big Mart sales dataset was loaded and explored using Pandas.

### 2. Data Preprocessing

* Handled missing values
* Processed categorical variables
* Converted features into a machine-learning-compatible format
* Removed/processed unnecessary information
* Prepared the dataset for model training

### 3. Exploratory Data Analysis

Exploratory analysis was performed to understand relationships between:

* Product attributes and sales
* Item MRP and sales
* Item visibility and sales
* Outlet characteristics and sales
* Outlet type and sales
* Outlet location and sales

### 4. Feature Engineering

Categorical and numerical features were transformed into suitable numerical representations for machine learning.

### 5. Model Development

Multiple regression approaches were explored, including:

* Ridge Regression
* Random Forest Regression
* Decision Tree Regression

The final deployed model is a **Decision Tree Regressor**.

### 6. Model Evaluation

The Decision Tree model was evaluated using regression metrics including:

| Metric                    |      Score |
| ------------------------- | ---------: |
| Mean Absolute Error (MAE) |   **0.31** |
| Mean Squared Error (MSE)  |   **0.53** |
| R² Score                  | **0.9596** |

The recorded results indicate an **R² score of 0.9596** on the evaluation reported in the project.

## 🤖 Final Model

**Algorithm:** Decision Tree Regressor

**Model Configuration:**

* `max_depth = 20`

The trained model is saved as:

```text
dtrs.pkl
```

The model is loaded by the Flask application and used to generate sales predictions.

## 🌐 Web Application

The project also includes a **Flask-based web application** for interacting with the trained model.

The application provides pages for:

* Home
* Login
* Dataset Upload
* Dataset Preview
* Sales Prediction
* Results
* Charts
* Model Performance

The prediction endpoint accepts input features, passes them to the trained Decision Tree model, and displays the predicted result.

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Matplotlib**
* **Flask**
* **Jupyter Notebook**
* **Pickle**
* **HTML/CSS/JavaScript**

## 📁 Project Structure

```text
Mini project/
│
└── sales prediction/
    ├── app.py
    ├── Accuracy.txt
    ├── data.csv
    ├── dtrs.pkl
    ├── requirements.txt
    │
    ├── model/
    │   ├── Train.csv
    │   ├── Test.csv
    │   ├── Untitled1.ipynb
    │   └── dtrs.pkl
    │
    └── static/
        └── assets/
```

## 📈 Results

The final Decision Tree Regression model achieved a recorded **R² Score of 0.9596**, with an MAE of **0.31** and MSE of **0.53** according to the project's evaluation results.

The project demonstrates how machine learning can be applied to retail sales forecasting and how a trained regression model can be integrated into a web application for making predictions.

## 🚀 Future Improvements

* Compare additional regression algorithms
* Perform advanced feature engineering
* Apply systematic hyperparameter tuning
* Improve model validation using cross-validation
* Add interactive data visualizations
* Improve the prediction interface
* Deploy the Flask application to a cloud platform
* Add an API endpoint for external applications
* Monitor model performance after deployment

## 💡 Applications

This type of sales prediction system can support:

* Demand forecasting
* Inventory planning
* Product-level sales estimation
* Retail analytics
* Store-level decision making
* Data-driven business planning

## 👨‍💻 Project

**Big Mart Sales Prediction**

A Machine Learning and Flask-based retail sales prediction project using historical Big Mart outlet data.
