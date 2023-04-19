# Bagging

<img src='bagging.png' align='right' width=450>

Bootstrap Aggregating, also known as bagging. 

Decision trees like CART select split points using a greedy algorithm that seeks to minimize a cost function, like the Gini index for classification. However, creating random sample of training data and choosing different split points will result different trees and different predictions. Combining these predictions from different models that have very different perspectives on the problem and this is where the power for bagging comes from [1].

Bootstrap method:

$$\bar{x} = \frac{1}{100} \times \sum_{i=1}^{100}x_i $$

## References

[1] [Master Machine Learning Algorithms](https://machinelearningmastery.com/master-machine-learning-algorithms/)
