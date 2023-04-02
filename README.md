# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Upload the file to your cell.
2. Type the required program.
3. Print the program. 
4. End the program.

## Program:
```python
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Rama E.K. Lekshmi
RegisterNumber: 212222240082
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.metrics import mean_absolute_error , mean_squared_error
df=pd.read_csv('student_scores.csv')
df.head()

df.tail()

X = df.iloc[:,:-1].values
X

y = df.iloc[:,-1].values
y

from sklearn.model_selection import train_test_split
X_train,X_test,y_train,y_test=train_test_split(X,y,test_size=1/3,random_state=0)

from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train,y_train)
y_pred=regressor.predict(X_test)

y_pred

y_test

plt.scatter(X_train,y_train,color="green")
plt.plot(X_train,regressor.predict(X_train),color="blue")
plt.title("Hours vs Scores (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()

plt.scatter(X_test,y_test,color="grey")
plt.plot(X_test,regressor.predict(X_test),color="purple")
plt.title("Hours vs Scores (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
*/
```

## Output:

![ml2 1](https://user-images.githubusercontent.com/118541549/229340935-a2ebcc8f-0520-4819-b175-4d7df1a5cbe2.png)
![ml2 2](https://user-images.githubusercontent.com/118541549/229340941-bbe479c1-1cfc-40f2-aca4-aa5690ad82ce.png)
![ml2 3](https://user-images.githubusercontent.com/118541549/229340950-d8a9ccf2-3ecc-470f-8a82-e0deed1b9a62.png)
![ml2 4](https://user-images.githubusercontent.com/118541549/229340951-cf9e78cd-8b9c-47c0-ace7-076da23dd078.png)
![ml2 5](https://user-images.githubusercontent.com/118541549/229340953-26bf19f8-8d5c-4fe0-9b4f-71a64704fe2e.png)
![ml2 6](https://user-images.githubusercontent.com/118541549/229340985-d230d8f8-2d2a-4b17-a9ff-3c01d6d159b6.png)
![ml2 7](https://user-images.githubusercontent.com/118541549/229340990-c3a9efc8-f1a6-4f0f-86f9-0abb47663efd.png)
![ml2 8](https://user-images.githubusercontent.com/118541549/229340995-caefa0bd-c622-439a-a9ae-e588092fb398.png)



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
