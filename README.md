# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fi

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is
1300cm cube.

## Program:
```
## Developed by: MOHAMED AZEEM N
## Reg.No: 22007405
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
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


![Screenshot (16)](https://user-images.githubusercontent.com/121040764/214200551-1a617bb7-86b4-4f0e-abfc-eeb89f501977.png)



## Result
Thus the multivariate linear regression is implemented and predicted the output using
python program.
