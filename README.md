# SGD-Regressor-for-Multivariate-Linear-Regression

## AIM:
To write a program to predict the price of the house and number of occupants in the house with SGD regressor.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Start and import the required libraries and dataset.
2.Split the dataset into input features X and target y.
3.Create an SGDRegressor model and fit it using the training data.
4.Predict the target values using the trained model.
5.Evaluate the model using Mean Squared Error (MSE) and display the results.

## Program:
```
/*
Program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor.
Developed by: DARSHINI R
RegisterNumber:  212225040054


import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model
import LinearRegression
from sklearn.datasets
import fetch_california_housing

data = { 'Size': [1000, 1200, 1500, 1800, 2000, 2200, 2500, 2700], 'Bedrooms': [2, 2, 3, 4, 4, 5, 5, 6], 'Age': [10, 8, 5, 3, 2, 2, 1, 1], 'Price': [45, 55, 70, 90, 100, 120, 135, 150], 'Rent': [15000, 18000, 22000, 28000, 32000, 35000, 40000, 45000]}
df = pd.DataFrame(data)
X = df[['Size', 'Bedrooms', 'Age']]Y = df[['Price', 'Rent']]
X_train, X_test, Y_train, Y_test = train_test_split( X, Y, test_size=0.2, random_state=42)
model = LinearRegression()model.fit(X_train, Y_train)
LinearRegression()
predictions = model.predict(X_test)
print("Predicted Values:")
print(predictions)
Predicted Values:[[ 53.96687697 17456.62460568] [ 116.5851735 35682.96529968]]
print("\nActual Values:")print(Y_test.values)
Actual Values:[[ 55 18000] [ 120 35000]]
new_house = [[1600, 3, 4]]prediction = model.predict(new_house)
print("\nPredicted House Price :", prediction[0][0], "Lakhs")
print("Predicted House Rent :", prediction[0][1], "Rs/month")

*/
```

## Output:

<img width="1180" height="414" alt="Screenshot 2026-08-20 112531" src="https://github.com/user-attachments/assets/ec4a692c-5bf6-4587-b85b-68802b59bca8" />
<img width="1155" height="322" alt="Screenshot 2026-08-20 112536" src="https://github.com/user-attachments/assets/2b35cd19-a8df-422d-b34b-8112c91c7c72" />



## Result:
Thus the program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor is written and verified using python programming.
