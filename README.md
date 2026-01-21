# **End-to-End Bike Rental Demand Prediction Using Machine Learning**

## **Project Overview**

This project implements an end-to-end machine learning pipeline to predict bike rental demand using historical usage data along with weather and temporal features. The goal is to understand the factors influencing bike rental patterns and build a reliable predictive model that can assist in urban mobility planning and resource optimization.

## **Features and Preprocessing**

**Numerical Features:** HOUR, TEMPERATURE, HUMIDITY, WIND_SPEED, VISIBILITY, DEW_POINT_TEMPERATURE, SOLAR_RADIATION, RAINFALL, SNOWFALL  

**Categorical Features:** SEASONS, HOLIDAY, FUNCTIONING_DAY  

## **Feature Engineering**

- Cyclic encoding of HOUR (sine and cosine)  
- Interaction feature between HOUR and TEMPERATURE  
- One-hot encoding of categorical variables  
- Scaling: StandardScaler applied to numerical features for model stability  

## **Modeling**

- **Regression Models:** Linear Regression (baseline), with potential extension to Random Forest or Gradient Boosting for improved performance  
- **Training and Testing:** Dataset split into training and test sets (80/20)  

## **Evaluation Metrics**

- Mean Squared Error (MSE)  
- R² Score  

## **Results**

Baseline Linear Regression model achieved:  

- **Mean Squared Error:** 176,918.98  
- **R² Score:** 0.58  

The model demonstrates moderate predictive ability and highlights the impact of weather and temporal features on bike rental demand.

## **Future Improvements**

- Experiment with more advanced models such as Random Forest, Gradient Boosting, or XGBoost  
- Include additional external features (e.g., holidays, special events, or real-time traffic data)  
- Perform hyperparameter tuning for better model performance  
- Explore log transformation of the target variable to reduce skewness  

## **Dataset**

The dataset includes hourly records of bike rentals, weather conditions, and other temporal features. All preprocessing and feature engineering steps are included in the code.

## **Usage**

1. Clone the repository  
2. Install required Python packages:  
```bash
pip install -r requirements.txt

#Run the preprocessing and modeling scripts

#To execute the preprocessing and model training, run the following command:

```bash
python bike_demand_prediction.py
