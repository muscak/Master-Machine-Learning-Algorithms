# Gaussian Naive Bayes

<img src='Gaussian Naive Bayes.png' align='right' width=450/>

Gaussian Naive Bayes assumes that each parameter (also called features or predictors) has an independent capacity of predicting the output variable. The combination of the prediction for all parameters is the final prediction, that returns a probability of the dependent variable to be classified in each group. The final classification is assigned to the group with the higher probability [1].

This is the extention of Naive Bayes which allows us working with real-valued attributes by assuming them in Gaussian (Normal) distribution which is the easiest to work with because you only need to estimate the mean and the standard deviation from your training data [2].

$$pdf(x, \mu, \sigma) = \frac{1}{\sigma \times \sqrt{2 \times \pi}} \times e^{-(\frac{(x-\mu)^2}{2 \times \sigma^2})}$$

Where $pdf(x)$ is the Gaussian PDF, $\mu$ and $\sigma$ are the mean and standard deviation calculated, $\pi$ is the numerical constant PI, $e$ is the numerical constant Euler’s number raised to power and $x$ is the input value for the input variable.

There are 2 steps to apply Gaussian Naive Bayes as regular Naive Bayes. Those are:
1. Calculating the probabilities for each class
2. Calculating the conditional probabilities but this time using the Gaussian Probability Density Function (PDF).

## 1. Calculate Class Probabilities

The probabilities of each class in the training dataset.

$$P(class = 1) = \frac{count(class=1)}{count(class=0) + count(class=1)}$$

$$P(class = 0) = \frac{count(class=0)}{count(class=0) + count(class=1)}$$

## 2. Calculate Conditional Probabilities 

The conditional probabilities of each feature value given each class value using Gaussian PDF.

$$y_i = P(pdf(x_1) | y = i)... \times ...P(pdf(x_p) | y = i) \times P(y = i)$$


---

[1] [Gaussian Naive Bayes Explained and Hands-On with Scikit-Learn](https://pub.towardsai.net/gaussian-naive-bayes-explained-and-hands-on-with-scikit-learn-4183b8cb0e4c)

[2] [Master Machine Learning Algorithms](https://machinelearningmastery.com/master-machine-learning-algorithms/)

[Practical Statistics for Data Scientists](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)
