# Linear Regression
Assumes that there is a linear relation between the inputs $(x)$ and output $(y)$.

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

## Gradient Desce


An error score can be used as a metric called Root Mean Squeared Error (RMSE) to measure the performance of the predictions. 

$$ RMSE = \sqrt{\frac{\sum\limits_{i=1}^{n} (p_i - y_i)^2}{n}} $$

where $p_i$ is the predicted value and $y_i$ is the actual value.
