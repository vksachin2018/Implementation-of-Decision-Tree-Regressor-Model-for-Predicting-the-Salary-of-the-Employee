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
![169694235-41a469cc-ff3e-4c56-b36c-029319ef1f94](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/409dd668-4b40-4a04-8ac4-5a1372185c16)
![169694238-85077655-4a64-4334-b451-997c7ea1937d](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/d388d212-e1bc-4890-9bc8-fde15143642c)
![169694242-dd7cae7b-50db-4864-96aa-ca8eb07514e3](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/85d259dd-98dc-4f4d-8dfc-97b0852345f2)
![169694248-eefed989-8fc7-4e80-b3af-992667d1936a](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/77cb0cff-9385-4904-b0f0-b9375d21ab32)
![169694252-b17fc5dd-22fd-46e0-b8de-991fd12528ed](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/9e55df11-f158-4e5d-98e6-2217f17c0fa4)
![169694255-16669af0-0ed0-416e-b387-d63f2f3e9dc3](https://github.com/vksachin2018/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149366019/cba6c1cf-4b28-429d-9a59-37d59e430a93)




## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
