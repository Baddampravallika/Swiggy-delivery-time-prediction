# 🚀 Swiggy Delivery Time Prediction

## 📌 Project Overview

This project uses Machine Learning to predict the estimated delivery time of Swiggy orders based on rider details, weather conditions, traffic, location, and order information. 
A Streamlit web application is developed to provide users with real-time delivery time predictions through an interactive interface.

## 🎯 Objective

To build a regression model that accurately predicts the delivery time of food orders, helping improve delivery planning and customer experience.

## ✨ Features

- Predicts delivery time in minutes
- Interactive Streamlit web application
- Uses both numerical and categorical features
- Real-time predictions with a trained ML model
- Simple and user-friendly interface

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Streamlit
- Pickle

## 📂 Project Structure

├── app.py
├── Swiggy-Delivery-Time-Prediction.ipynb
├── swiggy-project.pkl
├── swiggy_demographic.csv
├── requirements.txt
└── README.md

## ▶️ Installation

1. Clone the repository

git clone https://github.com/BaddamPravallika/Swiggy-delivery-time-prediction.git

2. Install the required packages

pip install -r requirements.txt

3. Run the application

streamlit run app.py

## 📊 Input Features

- Rider Details (Age, Rating, Vehicle Condition)
- Weather & Traffic
- City Information
- Order Details
- Distance
- Pickup Time
- Order Time


## 📈 Output

The model predicts the **estimated delivery time (in minutes)** based on the input details provided by the user.
