# *k*-Nearest Neighbors

<img src='0417red_WinInsider.jpeg' align='right' width=450/>

In statistics, the k-nearest neighbors algorithm (*k*-NN) is a non-parametric supervised learning method first developed by Evelyn Fix and Joseph Hodges in 1951[1] and later expanded by Thomas Cover[2]. It is used for classification and regression. In both cases, the input consists of the k closest training examples in a dataset[3].

The idea behind *k*NN is very simple. For each record to be classified or predicted:
1. Find *K* records that have similar features (i.e., similar predictor values).
2. For classification, find out what the majority class is among those similar records and assign that class to the new record.
3. For prediction (also called *k*NN regression), find the average among those similar records, and predict that average for the new record [4].

Neighbor is a record that has similar predictor values to another record. The Distance measures that sum up in a single number how far one record is from another. The most common way to measure the distance is to use Euclidean Distance.

$$Euclidean Distance (a,b) = \sqrt{\sum_{i=1}^{n}(a_i - b_i)^2}$$

Formula for Euclidean distance, derived from the Pythagorean theorem. With this formula, you can calculate the nearness of all the training data points to the data point you’re trying to label, and take the mean/mode of the k nearest neighbors to make your prediction [5].

---
## References

[1] [Discriminatory Analysis. Nonparametric Discrimination: Consistency Properties](https://apps.dtic.mil/dtic/tr/fulltext/u2/a800276.pdf)

[2] [Nearest neighbor pattern classification](http://ssg.mit.edu/cal/abs/2000_spring/np_dens/classification/cover67.pdf)

[3] [*k*-nearest neighbors algorithm](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)

[4] [Practical Statistics for Data Scientists](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)

[5] [Machine Learning for Humans](https://everythingcomputerscience.com/books/Machine%20Learning%20for%20Humans.pdf)
