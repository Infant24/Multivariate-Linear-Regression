# Implementation of Multivariate Linear Regression:

## Aim:

To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
 
## Algorithm:

### Step1
Import the necessary libraries and Read the dataset (car.csv).

### Step2
Select features (Weight, Volume) as x and Select target (CO2) as y.

### Step3
Create a Linear Regression model and Train the model using x and y.

### Step4
Obtain the model coefficients and intercept and Input new data for prediction (Weight, Volume).

### Step5
Predict CO2 using the trained model and Output the predicted CO2 value.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:/Users/admin/Downloads/car (1).csv")
x = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(x, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```

## Output:

<img width="1586" height="913" alt="image" src="https://github.com/user-attachments/assets/e8b64c0b-38bf-42da-9f20-62c49792b30e" />

## Result:

Thus the multivariate linear regression is implemented and predicted the output using python program.
