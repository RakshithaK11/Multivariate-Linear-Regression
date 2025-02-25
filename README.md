# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Get the independent variable X aand dependent variable Y.
### Step2
Import pandas as pd and also import linear_model from sklearn module.
### Step3
Read the CSV file which should be attached to the code runner.
### Step4
Give the commands to print LinearRegression and also the predicted CO2 for corresponding weights
### Step5
End the program
## Program:
~~~
'''
#Program to implement multivariate linear regression and predict the output.
#Developed by:RAKSHITHA K
#RegisterNumber:23003887
'''
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars (1).csv")
X=df[['Weight','Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

~~~
## Output:

### Insert your output

![image](https://github.com/RakshithaK11/Multivariate-Linear-Regression/assets/139336455/0d98e290-49c9-4783-959f-97d770002279)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
