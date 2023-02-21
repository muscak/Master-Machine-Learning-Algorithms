# Linear Regression
In statistics, linear regression is a linear approach for modelling the relationship between a scalar response and one or more explanatory variables (also known as dependent and independent variables). The case of one explanatory variable is called simple linear regression; for more than one, the process is called multiple linear regression*. Assumes that there is a linear relation between the inputs $(x)$ and output $(y)$.

The purpose of this study is to learn about simple and multiple linear regression using both traditional methods and sklearn library.

*[Wikipedia](https://en.wikipedia.org/wiki/Linear_regression#cite_note-Freedman09-1)


## Dataset
TV Marketing on [Kaggle](https://www.kaggle.com/datasets/devzohaib/tvmarketingcsv)

## Simple Linear Regression
It has a single input $(x)$ and the relation is represented by a line. 

$$y = \beta_0 + \beta_1×x$$

In higher dimensions when we have more than one input $(x)$, the line is called a **plane** or a **hyperplane**.

It calculates the $\beta_0$ and $\beta_1$ coefficients based on the below defined 2 formulas. 

$$\beta_1 = \dfrac{\sum\limits_{i=1}^{n} ((x_i - mean(x) × (y_i - mean(y))}{\sum\limits_{i=1}^{n} (x_i - mean(x))^2}$$

$$\beta_0 = mean(y) − \beta_1 × mean(x)$$

Then it predicts using the line equation mentioed above.

## Ordinary Least Squares

## Gradient Descent


An error score can be used as a metric called Root Mean Squeared Error (RMSE) to measure the performance of the predictions. 

$$ RMSE = \sqrt{\frac{\sum\limits_{i=1}^{n} (p_i - y_i)^2}{n}} $$

where $p_i$ is the predicted value and $y_i$ is the actual value.
