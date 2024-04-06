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
![319855596-f0907e87-5cd8-4cbf-90c6-af504e830ab2](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/0f1fbcae-6d82-437f-b198-722333e30863)
![319855664-a29039cb-cc26-4a7e-be70-2406f346f241](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/410e83b2-3485-49d7-9529-bfd71f42ad01)
![319855718-c5c471f5-ef23-4ab3-b510-68606602a4c0](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/4a184135-5214-48da-b422-b767dc93c34e)
![319855823-9eebc765-f4a5-4e35-bd64-7c2425478e7d](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/2a5cce7b-6240-4c69-a604-86542b0a0881)
![319855862-67589aa1-6fca-458c-a86d-04b3900c51df](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/c9899b64-e8ca-4c70-b5f2-da2bb1e9cfc6)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
