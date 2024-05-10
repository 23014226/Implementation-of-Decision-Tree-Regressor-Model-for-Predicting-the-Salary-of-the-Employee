# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program
2. Import pandas
3. Import Decision tree classifier
4. Fit the data in the model
5. Find the accuracy score
6. End the program

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: M GANESAN
RegisterNumber:  212223080013
*/
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred) 
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
```

## Output:

data.head()

![320274772-566ce1f5-3c40-401b-b4ec-105a6a986277](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/30e0ea93-162a-40f0-ab4c-b72e7a0f6f74)

data.info()

![320274784-0388ac9b-6f74-4055-a090-dca2d9c481b3](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/0acac481-b9b0-470e-9dca-fa93a568904a)

isnull() and sum()

![320274792-1ed92366-a8b8-4b6d-b7ce-6468749db08a](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/750a36df-6cb2-4f78-8b60-a5ca4c0b1eaf)

data.head() for salary

![320274801-6be8745a-1ffe-4589-a073-4a6c7bb7a2cd](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/9d0e0b70-1a1c-43aa-a834-59de48ad69cd)

MSE value

![320274809-a6e80f83-0987-44c9-bc5d-ad1d332cf868](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/d9185bef-9e93-4ae7-9be9-69e84119a353)

r2 value

![320274815-c36dd21f-a7cb-4091-a8af-0e376ab2931d](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/d19861b1-ba56-402d-be18-1ce9225fb40d)

data prediction

![320274820-33e7b744-fa7b-42a7-88e2-c3a2d6f1cc74](https://github.com/23014226/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/160568974/213aef08-cc05-448c-87d6-0161b59449d6)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
