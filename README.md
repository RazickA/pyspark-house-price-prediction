# House Price Prediction Using PySpark

This repository contains a **House Price Prediction** project, which utilizes **PySpark** to develop a machine-learning model for estimating home values based on historical data. The project employs big data techniques for preprocessing, exploratory analysis, and predictive modeling using Zillow Home Value Index (ZHVI) data.

---

## Project Overview

The **House Price Prediction** project aims to analyze real estate market trends and predict house prices using machine learning. The primary dataset used is the **Zillow Home Value Index (ZHVI)**, which contains monthly home values for various regions in the U.S. from **January 2000 to December 2024**.

### Key Features:
- **Data Preprocessing**: Handling missing values, transforming data, and engineering new features.
- **Exploratory Data Analysis (EDA)**: Understanding home price trends, regional variations, and correlations.
- **Machine Learning Models**: Implementing **Linear Regression, Random Forest, and Gradient Boosting** for price predictions.
- **Big Data Processing**: Leveraging **PySpark** for efficient computation on large datasets.

---

## Dataset

The dataset is sourced from **Zillow Research (ZHVI)** and contains:
- **RegionID**: Unique identifier for each geographical region.
- **SizeRank**: Rank of the region based on size.
- **RegionName**: Name of the city/metropolitan area.
- **RegionType**: Type of region (e.g., metro, county, state).
- **StateName**: The U.S. state where the region is located.
- **HomeValue (Target Variable)**: Monthly home values over the years.

---

## Technologies Used
- **Python** 
- **Apache PySpark** 
- **Pandas & NumPy** 
- **Matplotlib & Seaborn** 
- **Scikit-learn** 

---

## Exploratory Data Analysis (EDA)
We conducted **EDA** to identify key trends:
- **Yearly Home Price Trends**: Steady price growth with an acceleration post-2015.
- **Most Expensive Regions**: Top cities include **Jackson, WY**, **San Francisco, CA**, and **Santa Cruz, CA**.
- **Seasonal Trends**: Prices peak during summer months (June–August).
- **Urban vs. Rural Price Comparison**: Urban home prices are **45.36% higher** than rural prices.
- **Correlation Analysis**: Time-dependent trends and metropolitan market influence house prices.

---

## Machine Learning Models

### **Linear Regression**
- A simple model but performed poorly due to lack of non-linearity handling.

### **Random Forest Regression**
- An ensemble model that captures some non-linear relationships.
- Moderate performance with **lower RMSE** than Linear Regression.

### **Gradient Boosting Regression (Best Model)**
- Achieved **lowest RMSE (94,468.23)** and **highest R² (0.2712)**.
- Best alignment of predicted vs. actual home values.
- Recommended for **accurate home price predictions**.

---
