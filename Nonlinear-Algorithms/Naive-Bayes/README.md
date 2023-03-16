# Naive Bayes

Naive Bayes methods are a set of supervised learning algorithms based on applying Bayes’ theorem with the “naive” assumption of conditional independence between every pair of features given the value of the class variable[1]. Naive Bayes is a very simple classification algorithm that makes some strong assumptions about the independence of each input variable [2].

### Calculate Class Probabilities

The probabilities of each class in the training dataset.

$$P(class = 1) = \frac{count(class=1)}{count(class=0) + count(class=1)}$$

$$P(class = 0) = \frac{count(class=0)}{count(class=0) + count(class=1)}$$

### Calculate Conditional Probabilities 

The conditional probabilities of each feature value given each class value.

$$P(y = i|x_1, x_2, …, x_p) = \frac{P(y = i)P(x_1 | y = i)…P(x_p | y = i)}{P(y = 0)P(x_1 | y = 0)…P(x_p | y = 0) + P(y = 1)P(x_1 | y = 1)…P(x_p | y = 1)}$$


# Gaussian Naive Bayes


## References

[1] [Scikit-Learn](https://scikit-learn.org/stable/modules/naive_bayes.html#multinomial-naive-bayes)

[2] [Master Machine Learning Algorithms](https://machinelearningmastery.com/master-machine-learning-algorithms/)

[3] [Practical Statistics for Data Scientists](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)
