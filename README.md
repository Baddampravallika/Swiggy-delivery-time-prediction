# Swiggy Delivery Time Prediction

This project aims to predict the delivery time for food orders on the Swiggy platform using a machine learning model. Accurate ETA (Estimated Time of Arrival) prediction is critical for enhancing customer experience, reducing cancellations, and optimizing rider allocation.

## Business Problem
Swiggy processes millions of food-delivery journeys. Inaccurate ETAs lead to:
* Reduced customer trust and lower retention.
* Increased cancellations and refund costs.
* Operational inefficiencies and sub-optimal rider allocation.

## Objective
Develop a scalable, production-ready machine learning system that predicts delivery time (in minutes) at the moment of order placement, accounting for historical and real-time features.

## Dataset
The dataset includes various features such as:
- **Rider Metrics:** Age, ratings, vehicle condition, vehicle type.
- **Order Metrics:** Type of order, number of deliveries, pickup time.
- **Environmental/Temporal Metrics:** Traffic, weather, festival, weekend, time of day.
- **Geospatial Metrics:** Distance between restaurant and delivery location.

## Methodology
1. **Data Preprocessing:** Handled missing values using `SimpleImputer` (median for numerical, most frequent for categorical data) and managed categorical variables using `OneHotEncoder` and `OrdinalEncoder`.
2. **Feature Scaling:** Used `StandardScaler` to normalize numerical features.
3. **Model Building:** Experimented with multiple regression algorithms:
    - Linear Regression
    - K-Nearest Neighbors (KNN)
    - Decision Tree Regressor
    - Support Vector Machine (SVR)
    - Random Forest Regressor
    - **XGBoost Regressor** (Chosen for best performance)
4. **Optimization:** Used `GridSearchCV` and `Optuna` (Bayesian Optimization) to tune hyperparameters.

## Results
The final model, based on XGBoost, achieved strong predictive performance with an $R^2$ score of approximately **0.81** on the test set.

## Tech Stack
- Python
- Pandas
- Scikit-learn
- XGBoost
- Pickle (for model serialization)

## 📂 Project Structure
- `Swiggy-Delivery-Time-Prediction.ipynb`: Jupyter notebook containing the end-to-end data processing, modeling, and evaluation pipeline.
- `model.pkl`: Serialized model file for production use.
