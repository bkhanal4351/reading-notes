# Linear Regression in Python

In statistical modeling, regression analysis is a set of statistical processes for estimating the relationships between a dependent variable and one or more independent variables.

When Do You Need Regression?
- ypically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related.

# Linear Regression
- n statistics, linear regression is a linear approach for modelling the relationship between a scalar response and one or more explanatory variables. The case of one explanatory variable is called simple linear regression; for more than one, the process is called multiple linear regression.

Implementing Linear Regression in Python

Python Packages for Linear Regression
-The package NumPy is a fundamental Python scientific package that allows many high-performance operations on single- and multi-dimensional arrays. It also offers many mathematical routines. 

Simple Linear Regression With scikit-learn

There are five basic steps when you’re implementing linear regression:

1. Import the packages and classes you need.
2. Provide data to work with and eventually do appropriate transformations.
3. Create a regression model and fit it with existing data.
4. Check the results of model fitting to know whether the model is satisfactory.
5. Apply the model for predictions.


Multiple Linear Regression With scikit-learn

- You can implement multiple linear regression following the same steps as you would for simple regression.

Steps 1 and 2: Import packages and classes, and provide data

 First, you import numpy and sklearn.linear_model.LinearRegression and provide known inputs and output:

```import numpy as np
from sklearn.linear_model import LinearRegression

x = [[0, 1], [5, 1], [15, 2], [25, 5], [35, 11], [45, 15], [55, 34], [60, 35]]
y = [4, 5, 20, 14, 32, 22, 38, 43]
x, y = np.array(x), np.array(y)```


Step 3: Create a model and fit it

model = LinearRegression().fit(x, y)


Step 4: Get results

  ```>>> r_sq = model.score(x, y)
>>> print('coefficient of determination:', r_sq)
coefficient of determination: 0.8615939258756776
>>> print('intercept:', model.intercept_)
intercept: 5.52257927519819
>>> print('slope:', model.coef_)
slope: [0.44706965 0.25502548]```


Step 5: Predict response

  ```>>> y_pred = model.predict(x)
>>> print('predicted response:', y_pred, sep='\n')
predicted response:
[ 5.77760476  8.012953   12.73867497 17.9744479  23.97529728 29.4660957
 38.78227633 41.27265006]```  

Conclusion
You now know what linear regression is and how you can implement it with Python and three open-source packages: NumPy, scikit-learn, and statsmodels.

You use NumPy for handling arrays.

Linear regression is implemented with the following:

scikit-learn if you don’t need detailed results and want to use the approach consistent with other regression techniques
statsmodels if you need the advanced statistical parameters of a model
Both approaches are worth learning how to use and exploring further. The links in this article can be very useful for that.

When performing linear regression in Python, you can follow these steps:

Import the packages and classes you need
Provide data to work with and eventually do appropriate transformations
Create a regression model and fit it with existing data
Check the results of model fitting to know whether the model is satisfactory
Apply the model for predictions

notes taken from (https://realpython.com/linear-regression-in-python/#problem-formulation)

