# House Price Prediction Using Regression and Gradient Descent

## About This Project

This project applies supervised learning regression methods to predict house prices from real estate data. It walks through the full machine learning process, starting from raw data and ending with trained, evaluated, and compared models.

The goal is to study how different property features affect price, build several regression models of increasing complexity, and understand how well each model generalizes to new data.

---

## What This Project Covers

* Core ideas behind supervised learning and regression
* Exploring and visualizing the dataset
* Building a simple linear regression model
* Building a multiple linear regression model using all features
* Building a polynomial regression model for non linear patterns
* Evaluating models with standard regression metrics
* Coding gradient descent from scratch
* Comparing train and test scores to check for overfitting and underfitting

---

## Dataset

The dataset has 4200 property records with the following columns

| Column                | Meaning                          |
| --------------------- | --------------------------------- |
| house_id              | Unique id for each property        |
| area_sqft             | Total area of the house in sq ft   |
| bedrooms              | Number of bedrooms                 |
| bathrooms             | Number of bathrooms                |
| location_score        | Score rating the location quality  |
| age_years             | Age of the property in years       |
| distance_city_km      | Distance from the city center      |
| lot_size_sqft         | Size of the plot in sq ft          |
| has_garage            | Whether the house has a garage     |
| has_pool              | Whether the house has a pool       |
| renovation_years_ago  | Years since the last renovation    |
| house_price_inr       | Price of the house in rupees, this is the target |

---

## Tools and Libraries

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit Learn

---

## Notebook Structure

### Part A, Concepts

Short explanations of supervised learning, regression, and the assumptions behind linear regression.

### Part B, Exploring the Data

Loading the dataset, checking data types, checking for missing values, looking at correlations, and plotting relationships between features and price.

### Part C, Simple Linear Regression

A model that predicts price using only the area of the house. Includes a fitted line plot and interpretation of the slope and intercept.

### Part D, Evaluating the Simple Model

The model is scored using Mean Squared Error, Mean Absolute Error, Root Mean Squared Error, R squared, and Adjusted R squared. Residuals are plotted to check the assumptions.

### Part E, Multiple Linear Regression

A model trained on all the property features together, compared against the simple model.

### Part F, Polynomial Regression

A degree two polynomial model to capture curved relationships that a straight line cannot represent.

### Part G, Gradient Descent From Scratch

A manual implementation of gradient descent on the standardized area feature, showing how the weight and bias are updated step by step until the cost stops decreasing.

### Part H, Checking for Overfitting and Underfitting

Train and test scores for each model are compared side by side to see how well each one generalizes.

### Part I, Conclusions

A short summary of what worked best and why.

---

## Visualizations Included

* Correlation heatmap of all features
* Area vs price and age vs price scatter plots
* Pair plot of key features
* Regression line for the simple model
* Residual plots
* Gradient descent cost curve
* Bar chart comparing R squared across models

---

## Models Built

**Simple Linear Regression**
Uses only area to predict price. Easy to interpret but limited in accuracy.

**Multiple Linear Regression**
Uses all available features, giving a more complete picture of what drives price.

**Polynomial Regression**
Adds squared and interaction terms to catch non linear effects.

**Gradient Descent (from scratch)**
A hand coded version of linear regression that learns the weight and bias through repeated small updates instead of using a closed form solution.

---

## Evaluation Metrics Used

| Metric      | What it tells you                         |
| ----------- | ------------------------------------------ |
| MSE         | Average of the squared errors              |
| MAE         | Average of the absolute errors             |
| RMSE        | Error in the same units as price           |
| R2 Score    | How much of the variation in price is explained |
| Adjusted R2 | R2 adjusted for the number of features used |

---

## Key Takeaways

* The dataset was fairly clean with no major missing value problems
* Area and location score had the strongest relationship with price
* Multiple linear regression clearly outperformed the simple single feature model
* Polynomial regression improved R2 slightly further but needs to be checked for overfitting
* The gap between train and test scores stayed small across models, which is a good sign for generalization
* The gradient descent cost curve dropped quickly and then flattened, showing the model converged correctly

---

## What I Practiced

* Exploratory data analysis
* Data visualization
* Building and comparing regression models
* Calculating and interpreting evaluation metrics
* Implementing gradient descent manually
* Diagnosing overfitting and underfitting
