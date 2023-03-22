# Gaussian Naive Bayes

<img src='Gaussian Naive Bayes.png' align='right' width=450/>

Gaussian Naive Bayes assumes that each parameter (also called features or predictors) has an independent capacity of predicting the output variable. The combination of the prediction for all parameters is the final prediction, that returns a probability of the dependent variable to be classified in each group. The final classification is assigned to the group with the higher probability [1].

$$pdf(x, \mu, \sigma) = \frac{1}{\sqrt{2 \times \pi} \times \sigma} \times e^-(\frac{(x-\mu)^2}{2 \times \sigma^2})$$

---
[1] [Gaussian Naive Bayes Explained and Hands-On with Scikit-Learn](https://pub.towardsai.net/gaussian-naive-bayes-explained-and-hands-on-with-scikit-learn-4183b8cb0e4c)

[Practical Statistics for Data Scientists](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)

[Master Machine Learning Algorithms](https://machinelearningmastery.com/master-machine-learning-algorithms/)
