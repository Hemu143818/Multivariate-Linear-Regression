# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.
### Step2
Read the csv file.
### Step3
Get the value of X and y variables.
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 1000kg, and the volume is 1390cm3.
### Step6
Print the predicted output.
## Program:
```
\*
#Multivariate Linear Regression
#Developed by : PRITHIVIRAJAN V
#Register Number : 212223100042
\*
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('/content/cars (1) (1).csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
print("Amount",regr.predict([[3300,1300]]))
```
## Output:

![image](https://github.com/Prithivirajan2911/Multivariate-Linear-Regression/assets/147020085/e875da86-378f-40dd-b8c7-f3f4c0ea7342)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
