# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step-1 import pandas as pd.

### Step-2 Read the csv file.

### Step-3 Get the value of X and y variables

### Step-4 Create the linear regression model and fit.

### Step-5 Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
## Program:
```
Developed by : PRAGATHEESWARAN K
Reg No : 212225040310
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:
<img width="1039" height="98" alt="image" src="https://github.com/user-attachments/assets/c471f9cb-0609-4cd8-9d02-fe5b83c00f64" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
