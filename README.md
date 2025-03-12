Implementation of Univariate Linear Regression
AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

Equipments Required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Jupyter notebook
Algorithm
Get the independent variable X and dependent variable Y.
Calculate the mean of the X -values and the mean of the Y -values.
Find the slope m of the line of best fit using the formula.
image

4. Compute the y -intercept of the line by using the formula:
image

5. Use the slope m and the y -intercept to form the equation of the line. 6. Obtain the straight line equation Y=mX+b and plot the scatterplot.
Program:
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: AANKARSH
RegisterNumber:  212223233001
*/
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
denom=8,
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-m*x_mean
print(m,b)
y_predicted=m*x+b
print(y_predicted)
plt.scatter(x,y)
plt.plot(x,y_predicted,color='red')
plt.show()
Output:

![ml ex 1 img 1](https://github.com/user-attachments/assets/b472d43d-11e5-4538-9072-7f4806ca5a5f)


Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
