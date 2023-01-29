# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1

import pandas from library
Step2

import linear_model from sklearn
Step3

Read the csv file usingpandas library
Step4

Enter the parameters of the linear function.
Step5

Print the parameters of the linear function.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)





```
## Output:

![WhatsApp Image 2023-01-29 at 19 40 47](https://user-images.githubusercontent.com/118660461/215332493-9964737c-c927-4984-8f10-05d88c4dd96c.jpg)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
