# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packagesprint the present data

2.print the present data

3.print the null value

4.using decisiontreeRegressor, find the predicted values,mse,r2

5.print the result 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: gokul sachin .k
RegisterNumber:  212223220025

import pandas as pd
data=pd.read_csv("/content/Salary_EX7.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
x_train
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
from sklearn.tree import DecisionTreeRegressor, plot_tree
import matplotlib.pyplot as plt
clf=DecisionTreeRegressor(criterion='gini')
plt.figure(figsize=(20,8))
plot_tree(dt,feature_names=x.columns,filled=True)
plt.show()

```

## Output:
![280373820-1db1e938-9d9d-4121-9f63-6dd77e01f1ac](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/ce5ec843-6cda-4d92-aadb-0b635c4932a0)
![280373948-81134bd4-85bb-4809-babd-90fb83770104](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/763eb218-8b2a-4cb9-b7e0-ca941a6565e1)
![280378600-54e9c59b-69ce-4599-924e-0d7cd7ba3d61](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/79f7b39f-2199-4ae9-858e-0b092cf5a0a7)

![280378922-3ae61255-5974-4c9d-8412-3ae45d8cf60d](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/f32d1200-9ac7-45b4-8a1c-16b76f9f95b7)
![280379034-199eec7f-580a-4b12-81eb-7a617e90ba18](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/b03e3079-e9bf-45cb-ba45-b0e425fec092)
![280379192-991437fc-9ae1-4435-8a9d-b1f6cc5a05a1](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/efabf57d-455e-448a-b170-2ee9cfe5cc98)
![280379312-085838db-697d-45e0-b61c-33c5428403ae](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/82f38c37-1b0b-478d-9935-0f66d4b03b44)





## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
