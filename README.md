# Implementation of Multivariate Linear Regression
## Aim:
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 : import pandas as pd.
### Step2 : Read the C SV file.
### Step3 : Get the value of x and y variables.
### Step4 : Create the linear regression model and fit.
### Step5 : Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

## Program:
```
Developed by: SRI SAI PRIYA.S
Reference number: 22006141

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[["weight","volume"]]
y=df['co2']
regr=linear_model.linearregression()
regr.fit(x,y)
print("Coefficient",regr.coef_)
print("Intercept".regr.intercept_)
predictedco2=regr.predict([[3300,1300]])
print("predicted co@ for the coressponding weight and volume",predictedco2)
```
## Output:
![output](/mul.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
