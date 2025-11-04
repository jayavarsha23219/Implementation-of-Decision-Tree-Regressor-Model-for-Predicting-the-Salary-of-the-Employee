# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the standard libraries.

2. Upload the dataset and check for any null values using .isnull() function.

3. Import LabelEncoder and encode the dataset.

4. Import DecisionTreeRegressor from sklearn and apply the model on the dataset.

5. Predict the values of arrays.

6. Import metrics from sklearn and calculate the MSE and R2 of the model on the dataset.

7. Predict the values of array.

8. Apply to new unknown values.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: JAYAVARSHA T  
RegisterNumber: 212223040075

import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position", "Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size=0.2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train, y_train)
y_pred = df.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test, y_pred)
mse
r2 = metrics.r2_score(y_test, y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
<img width="456" height="248" alt="image" src="https://github.com/user-attachments/assets/906dfe56-9e0b-4eb7-bebb-5dbffa10e525" />
<img width="425" height="237" alt="image" src="https://github.com/user-attachments/assets/acb7ce4d-c9d5-4437-a5a6-6c4ffd01421b" />
<img width="297" height="228" alt="image" src="https://github.com/user-attachments/assets/622cf7c1-84a1-48ae-88dc-7df46704755e" />
<img width="512" height="313" alt="image" src="https://github.com/user-attachments/assets/c0be6b78-7647-458e-a2c6-9df30c2ba841" />
<img width="471" height="157" alt="image" src="https://github.com/user-attachments/assets/94df1436-1736-43ae-81a5-545212edeced" />
<img width="632" height="107" alt="image" src="https://github.com/user-attachments/assets/236c5c43-7afc-4fec-b07b-0690ad834e8e" />

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
