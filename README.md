# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1: Import libraries (numpy, matplotlib, LinearRegression).
Step 2: Define dataset X, Y.
Step 3: Fit linear regression model.
Step 4: Extract slope & intercept.
Step 5: Predict marks for user input.
Step 6: Plot scatter points & regression line.

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Guru Prasad D.R.
RegisterNumber:  212225040104

import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

X=np.array([1,2,3,4,5]).reshape(-1,1)
Y=np.array([35,50,65,70,85])
model=LinearRegression()

model.fit(X,Y)

m=model.coef_[0]
b=model.intercept_

print("Slope(m):",m)
print("Intercept(b):",b)

x_value=float(input("Enter hours studied:"))
prec_mark=model.predict([[x_value]])
print("Predicted mark:",prec_mark[0])

y_pred=model.predict(X)

plt.scatter(X,Y,label="Hours studied")
plt.plot(X,y_pred,label="Marks scored")
plt.xlabel("X")
plt.ylabel("Y")
plt.legend()
plt.title("Simple linear regression using sklearn")
plt.show()
*/
```

## Output:
![simple linear regression model for predicting the marks scored](sam.png)
<img width="860" height="673" alt="image" src="https://github.com/user-attachments/assets/d2db9df5-b1b4-4b49-9df0-af357d0f7fb2" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
