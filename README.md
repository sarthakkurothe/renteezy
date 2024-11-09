# Renteezy

**Renteezy** is an all-in-one solution designed to help tenants find rental properties more efficiently. This application allows users to input their desired house features (such as amenities and number of bedrooms) for rent predictions in metro cities. It provides graphical analyses to solve real-world rental issues, with a focus on helping new tenants find ideal rentals in big cities.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Installation](#installation)

## Features

- Predict rental prices based on selected features (e.g., number of bedrooms, amenities).
- Visual analysis of rental data in metro cities.
- User-friendly interface tailored for tenants looking for rental properties in big cities.
- Solves rental issues by providing convenience and insights for tenants.

## Technologies Used

- Python
- Numpy
- Pandas
- PostgreSQL
- Scikit-Learn
- Plotly
- Matplotlib
- Seaborn
- Streamlit

## Getting Started

To get a local copy up and running, follow these steps.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/sarthakkurothe/renteezy.git
   ```

2. Create virtual environment:

   ```bash
    python -m venv venv
    venv\Scripts\activate
   ```

3. Install the required packages:

  ```bash
    pip install -r requirements.txt
 ```

4. Run the Streamlit app:

  ```bash
  streamlit run app.py
  ```

## Machine Learning Regression Model

### 1. Algorithm Assessment
The dataset is split into training and testing subsets, where multiple regression algorithms are evaluated based on R² scores to identify the most accurate model.

### 2. Algorithm Selection
After testing various models, **Random Forest Regressor** is chosen for its balance of interpretability and performance, as well as its lack of overfitting compared to other models like Gradient Boosting and XGB Regressors.

### 3. Hyperparameter Tuning
Using grid search and cross-validation, the model's hyperparameters are fine-tuned for optimal predictive accuracy and robustness.

### 4. Model Evaluation
The model’s performance is assessed using key metrics: **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, **Root Mean Squared Error (RMSE)**, and **R-squared (R²)** to ensure accuracy in rental price prediction.

### 5. Model Persistence
The trained model is saved as a pickle file, allowing it to be reused efficiently for future rental predictions.

---

## Exploratory Data Analysis (EDA) - Streamlit Application

### 1. Data Migration to SQL
Predicted data is stored in a PostgreSQL database for structured storage and easy retrieval using SQL queries.

### 2. Property Type (BHK) Analysis
An analysis of average rent by property type (BHK) provides insights into how configurations impact rental prices.

### 3. Lease Type and Property Characteristics
Comparing rent across lease types, property size, and age highlights market trends and dynamics.

### 4. Amenities and Features
The impact of amenities like gyms, pools, and ACs on rent is analyzed, providing insights into tenant preferences and property management strategies.

### 5. Location and Structural Factors
Factors such as parking, floor arrangement, balconies, and negotiability are examined for their influence on average rents.

### 6. Interactive Prediction
An interactive feature lets users input property parameters to predict rent using the pre-trained model, allowing exploration of different configurations for tailored forecasts.

---
