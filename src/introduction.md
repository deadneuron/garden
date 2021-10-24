# Introduction

Artificial neural networks are computing systems inspired by the biological neural networks that constitute our brains. They are made up of many connected nodes called neurons, usually organized into hierarchical layers.

![](../images/intro-nn.svg)

The connections between neurons typically have a weight associated with them that changes through learning. Neurons take these weighted inputs from other neurons and computes a non-linear function on the sum.

$$
y = \sigma(\sum{w_i x_i})
$$

These neurons are then composed into layers. The overall network can be thought of as a combination of function composition and matrix multiplication with tunable parameters.

$$
g(x) := f_1  (w_1 f_2(w_2 f_3 (...)))
$$

Learning happens by passing the training data through the network and optimizing the parameters to reduce some error function. Mean Suared error is a popular one.

$$
MSE = \frac{1}{N} \sum{(t - y)^2}
$$