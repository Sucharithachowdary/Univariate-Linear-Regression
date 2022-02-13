# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
import numpy as np

x = np.array(eval(input()))
y = np.array(eval(input()))

# mean
x_mean=np.mean(x)
y_mean=np.mean(y)
#(x-xi) & (yi-y)
num=0
deno=0

for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    deno+=(x[i]-x_mean)**2
m=num/deno
b=y_mean-m*x_mean
print(m,b)
y=m*x+b
print(y)

```
## Sample Input and Output
![linear regression](https://user-images.githubusercontent.com/94166007/153746061-9ef96bd6-bf09-4966-b8c6-67d111344c11.PNG)

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
