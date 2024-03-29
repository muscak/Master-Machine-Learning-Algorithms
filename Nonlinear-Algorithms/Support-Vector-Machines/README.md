# Support Vector Machines (SVM)

In machine learning, support vector machines (SVMs, also support vector networks) are supervised learning models with associated learning algorithms that analyze data for classification and regression analysis [1]. Before going deep in SVM, there are 2 things that must be learned.

<p align="center">
  <img src='svm.jpeg' width='350' alt='Support Vector Machines' />
</p>
<p align="center">
    <b>Fig. 1: Support Vector Machines [4]</b>
</p>

## 1. Maximal-Margin Classifier

Maximal-Margin Classifier is a hypothetical classifier and it explain how SVM works. The features (inputs) in your data may form a n-dimensional space. 

A hyperplane is a line that splits the input variable space by their classes. If the we have 2 inputs which mean that we have 2 dimentional space and the hyperplane can be visualized as a line as shown in the above image. This line can be defined as below formula:

$$B_0 + (B_1 × X_1) + (B_2 × X_2) = 0$$

Where $X_1$ and $X_2$ are the two input variables, $B_1$ and $B_2$ are the coefficients that determine the slope of the line and $B_0$ the intercept. The coefficients and the intercept are found by the learning algorithm. The distance between the line and the closest data points are called as the margin. The best or optimal line that can separate the classes is the line that has the largest margin. This is called the Maximal-Margin hyperplane. The margin is calculated as the perpendicular distance from the line to only the closest points. These points are called the **support vectors**. The hyperplane is learned from training data using an **optimization procedure that maximizes the margin**. 

So Maximal Margin Classifiers are super sensitive to outliers in the training data and that makes them pretty lame [2].

## 2. Soft Margin Classifier

In practice, real data is messy and cannot be separated perfectly with a hyperplane. The constraint of maximizing the margin of the line that separates the classes must be relaxed [1]. Choosing a threshold that allows misclassifications is an example of the Bias/Variance Tradeoff that plagues all of machine learning. When we allow misclassifications, the distance between the observations and the threshold is called a Soft Margin [2].

## 3. Kernels

In order to make the mathematics possible, Support Vector Machines use something called Kernel Functions to systematically find Support Vector Classifiers in higher dimensions [2]. The kernel defines the similarity or a distance measure between new data and the support vectors [1].

### 3.1. Linear Kernel SVM
The dot product is the similarity measure used for linear kernel because the distance is a linear combination of the inputs.

$$K(x, x_i) = \sum(x \times x_i)$$

### 3.2. Polynomial Kernel SVM
Another kernel method is polynomial one which allows for curved lines in the input space. If $d=1$, this is the same as linear kernel. It computes relationships between pairs of observations. $x$ and $x_i$ refer to the two observations we want to calculate the high dimensional relationship for. And $d$ determines the degree of polynomial which is determined using cross validation.

$$K(x, x_i) = 1 + \sum(x \times x_i)^d$$

### 3.3. Radial Kernel SVM
The radial kernel is very local and can create complex regions within the feature space, like closed polygons in a two-dimensional space [1]. It uses infinite dimensions for classification. It behaves like weighted nearest neighbor model. The closest observations (nearest neighbors) have a lot of influence on classifying the new observations [2]. 

$$K(x, x_i) = e^{-\gamma \times \sum(x - x_i)^2}$$

In the below image, you can see the comparison of the different kernels using the Iris dataset.

<p align="center">
  <img src='sphx_glr_plot_iris_svc_001.png' width=550 align='center' alt='Support Vector Machine - Kernels' />
</p>
<p align="center">
    <b>Fig. 2: Different Kernels [3]</b>
</p>

In summary, when we have 2 classes, but no obvious linear classifier that seperates them in a nice way, **SVM** work by moving the data into a relatively high dimensional space and finding a relatively high dimensional **Support Vector Classifier** that can effectively classify the observations [2]. 

## References

[1] [Support vector machine](https://en.wikipedia.org/wiki/Support_vector_machine)

[2] [Support Vector Machines Part 1 (of 3): Main Ideas!!!](https://www.youtube.com/watch?v=efR1C6CvhmE)

[3] [Support Vector Machines](https://scikit-learn.org/stable/modules/svm.html)

[4] [Support Vector Machine (SVM)](https://nl.mathworks.com/discovery/support-vector-machine.html)
