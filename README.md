# Implementation of Multivariate Linear Regressio
## date: 13-05-2025
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
#Developed by hemanth yadav
#Register Number : 212224100033
\*
 import pandas as pd
 from sklearn import linear_model
 df = pd.read_csv("car.csv")
 X = df[['Weight', 'Volume']]
 y = df['CO2']
 regr = linear_model.LinearRegression()
 regr.fit(X, y)
 print('Coefficients:', regr.coef_)
 print('Intercept:',regr.intercept_)
 predictedCO2 = regr.predict([[3300, 1300]])
 print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![Screenshot 2025-05-13 211706](https://github.com/user-attachments/assets/772740fe-1944-4c14-95ba-2512b9a406a5)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
