# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

## Step1
Import Pandas library and linear_model from sklearn using import statement.

## Step2
Read the given csv file using read_csv() method.

## Step3
Create two arrays, independent array x with two classes and dependent array y with one class. Find the regression of x and y using linear_model.LinearRegression() method and fit x and y usind .fit() method.

## Step4
Find the coefficients using .coef_ and intercept using .intercept_ .

## Step5
Predict the liner regression using regr.predict() method and display the result.

## Program:
```
import pandas as pd
from sklearn import linear_model 
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)```



```
## Output:
![image](https://github.com/DEVADARSHAN2/Multivariate-Linear-Regression/assets/119432150/11e97eea-b21f-4383-9cbb-e05c142cfd63)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
