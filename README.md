# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Start and import the required libraries — pandas for data handling and linear_model from sklearn for regression.

### Step2
Load the dataset from the CSV file using pd.read_csv() and store it in a DataFrame df.

### Step3
Select features and target:
Set X = [['Weight', 'Volume']] (independent variables).
Set y = ['CO2'] (dependent variable).

### Step4
Create a Linear Regression model using linear_model.LinearRegression() and store it in regr.

### Step5
Train the model using regr.fit(X, y) and display the model’s coefficients and intercept.

### Step6
Predict CO2 value for a given weight and volume using regr.predict() and print the predicted result.

## Program:
```
Designed By : B Prabhanjan
Register No : 212225040305

import pandas as pd
from sklearn import linear_model
df=pd.read_csv(r"C:\Users\acer\Desktop\car(1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))




```
## Output:

![alt text](<Screenshot 2026-03-23 230012.png>)




## Result


Thus the multivariate linear regression is implemented and predicted the output using python program.