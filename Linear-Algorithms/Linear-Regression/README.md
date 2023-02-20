# Linear Regression
Assumes that there is a linear relation between the inputs $(x)$ and output $(y)$.

## Dataset
TV Marketing on [Kaggle](https://www.kaggle.com/datasets/devzohaib/tvmarketingcsv)

## Simple Linear Regression
It has a single input $(x)$ and the relation is represented by a line. 

$$
  y = \beta_0 + \beta_1×x
$$ (1)

In higher dimensions when we have more than one input $(x)$, the line is called a **plane** or a **hyperplane**.

It calculates the $\beta_0$ and $\beta_1$ coefficients based on the below defined 2 formulas. 
$$\beta_1 = \dfrac{\sum\limits_{i=1}^{n} ((x_i - mean(x) × (y_i - mean(y))}{\sum\limits_{i=1}^{n} (x_i - mean(x))^2}$$

$$\beta_0 = mean(y) − \beta_1 × mean(x)$$



## Ordinary Least Squares

## Gradient Desce
