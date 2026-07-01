HOUSE PRICE REGRESSION PROJECT

OVERVIEW
This project predicts house prices using regression techniques in Python. It uses a dataset of 4200 houses with features like area, bedrooms, bathrooms, location score, age, distance from city, lot size, garage, pool, and renovation history. The target value to predict is house price in INR.

FILES IN THIS PROJECT
House_Price_Regression_Project.ipynb - the main Jupyter notebook with all code, charts, and explanations
RealEstate_HousePrice_Dataset_4200.csv - the dataset used for training and testing the models

HOW TO RUN THIS PROJECT
1. Install Python and Jupyter Notebook if not already installed
2. Install the required libraries by running this command
   pip install numpy pandas matplotlib seaborn scikit-learn
3. Create a folder named data in the same location as the notebook
4. Place the CSV file inside the data folder and rename it to house_data.csv
   The notebook expects the file at data/house_data.csv
5. Open the notebook and run all cells from top to bottom

WHAT THE NOTEBOOK COVERS
Part A explains supervised learning and regression concepts
Part B loads and explores the dataset, checks for missing values, and visualizes relationships between features and price
Part C builds a simple linear regression model using only house area to predict price
Part D evaluates the simple model using MSE, MAE, RMSE, R2, and adjusted R2
Part E builds a multiple linear regression model using all available features
Part F builds a polynomial regression model to capture curved relationships
Part G implements gradient descent from scratch to show how a model learns step by step
Part H compares training and testing scores to check for overfitting or underfitting
Part I summarizes the findings and conclusions

MAIN FINDINGS
Multiple linear regression performs better than simple linear regression because it uses more information about each house
Polynomial regression improves results slightly further by capturing non linear patterns
The gradient descent section shows the cost decreasing over time, proving the model is learning correctly
The gap between training and testing scores is small, which means the models generalize well and are not overfitting

REQUIREMENTS
Python 3
Jupyter Notebook or JupyterLab
numpy
pandas
matplotlib
seaborn
scikit-learn

NOTES
This project is for learning purposes and demonstrates core regression concepts including data preprocessing, model training, evaluation metrics, and gradient descent optimization
