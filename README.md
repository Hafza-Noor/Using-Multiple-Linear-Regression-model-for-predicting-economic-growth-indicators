# Using-Multiple-Linear-Regression-model-for-predicting-economic-growth-indicators
This project analyzes global economic indicators and builds a Multiple Linear Regression model to predict a country's Gross Domestic Product (GDP). 
The dataset contains several key macroeconomic variables such as Population, Gross National Income (GNI), Imports, Exports, and Gross Capital Formation.
The goal is to identify which indicators most strongly influence GDP and how accurately they can predict economic performance.

 ### Steps Performed
#### 1. Data Loading and Selection

The dataset was imported from a CSV file named Global_Economy_Indicators.csv.

Selected important columns:Country

Year

Population

Gross National Income(GNI) in USD

Imports of goods and services

Exports of goods and services

Gross capital formation

Gross Domestic Product (GDP)

#### 2. Data Cleaning

Missing values were identified using df.isnull().sum().

Columns with missing values were handled by replacing them with column means using:
#### 3. Exploratory Data Analysis (EDA)

A correlation heatmap was plotted to visualize relationships between indicators.
It showed strong positive correlations between GDP, GNI, and trade variables.

The dataset demonstrated meaningful linear patterns suitable for regression modeling.

#### 4. Regression Modeling

Model Used: LinearRegression from sklearn.linear_model

Target Variable: Gross Domestic Product (GDP)

Independent Variables: Population, GNI, Imports, Exports, and Capital Formation.

The dataset was split into training and testing sets using:
#### 5. Model Evaluation

Metrics Used:

R² Score: 0.9998

Mean Squared Error (MSE): 1.46e+20

The R² score shows that the model explains over 99% of the variance in GDP, indicating a very strong fit.

#### 6. Residual Analysis

Histogram and Q-Q Plot of residuals were generated to check normality.
The residuals were approximately centered around zero but showed minor deviations, suggesting possible non-linear relationships.

Checking residuals ensures model reliability and validates the linear regression assumptions.

#### 7. Feature Importance

Coefficients from the regression model were analyzed and visualized.
Interpretation:
Population has the highest impact on GDP, followed by GNI.
This indicates that demographic and income-related factors play the most crucial role in determining a country's economic output.

### Visualizations Included

Correlation Heatmap

Actual vs Predicted GDP Plot

Residual Histogram and Q-Q Plot

Feature Importance Bar Chart

### Conclusion

This regression model effectively predicts GDP using key economic indicators.
The analysis highlights that Population and GNI are the strongest predictors of economic growth.
Future improvements could include:

Standardizing the data before regression for better coefficient comparison.

Testing advanced models such as Ridge, Lasso, or Random Forest Regressor.

Expanding to time-series or cross-country forecasting using Monte Carlo Simulation or ARIMA.

## Hafza Noor
### hafzanoor3106@gmail.com
### https://www.linkedin.com/in/hafza-noor-a40ab1236/
