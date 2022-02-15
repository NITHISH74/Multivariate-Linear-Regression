# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.


### Step2
Import Linear_model from sklearn.


### Step3
Read the csv file using pandas library.


### Step4
Enter the parameters of the linear function.


### Step5
Print the parameters of the linear function.


## Program:
```
# Name: NITHISHWAR S
# Ref.no: 21002766

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
print("predicted CO@ for the corresponding weight and volume",predictedCO2)

```
## Output:

![image](https://user-images.githubusercontent.com/94164665/154081087-e2b4bbc2-a9e7-46e7-849f-33339c2c07e3.png)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
