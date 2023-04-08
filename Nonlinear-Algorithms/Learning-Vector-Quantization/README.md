# Learning Vector Quantization (LVQ)

<img src='LVQ.png' align='right' width=350 alt='Learning Vector Quantization (LVQ)'/>

In computer science, learning vector quantization (LVQ) is a prototype-based supervised classification algorithm[1]. LVQ is a family of algorithms for statistical pattern classification, which aims at learning prototypes (codebook vectors) representing class regions. The class regions are defined by hyperplanes between prototypes, yielding Voronoi partitions[2].

A codebook vector is a list of numbers that have the same input and output attributes as your training data. The model representation is a fixed pool of codebook vectors, learned from the training data. They look like training instances, but the values of each attribute have been adapted based on the learning procedure. In the language of neural networks, each codebook vector may be called a neuron, each attribute on a codebook vector is called a weight and the collection of codebook vectors is called a network [3].

Predictions are made for a new instance by searching through all codebook vectors for the $k$ most similar instances and summarizing the output variable for those $k$ instances. For classification this is the mode (or most common) class value. Typically predictions are made with $k$ = 1, and the codebook vector that matches is called the Best Matching Unit (BMU). To calculate the most similar unit, we need a distance measure.

$$Euclidean Distance (a,b) = \sqrt{\sum_{i=1}^{n}(a_i - b_i)^2}$$

The amount that the vector is moved is controlled by an algorithm parameter called the learning rate ($LearningRate$). For example, the input variable ($x$) of a codebook vector is moved closer to the training input value ($t$) by the amount in the LearningRate if the classes match as follows:

$$x = x + LearningRate × (t − x)$$

The opposite case of moving the input variables of a codebook variable away from a training instance is calculated as:

$$x = x - LearningRate × (t − x)$$

---
## References

[1] [Learning Vector Quantization](https://en.wikipedia.org/wiki/Learning_vector_quantization)

[2] [A Review of Learning Vector Quantization Classifiers](https://arxiv.org/pdf/1509.07093.pdf)

[3] [Master Machine Learning Algorithms](https://machinelearningmastery.com/master-machine-learning-algorithms/)
