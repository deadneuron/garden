# Neurons

Neurons are the fundamental building blocks of neural networks, inspired by their biological counterparts. They work by taking a weighted some of inputs from other neurons and passing that through some nonlinear activation function.


![Neuron](https://upload.wikimedia.org/wikipedia/commons/b/b0/Artificial_neuron.png)


$$
out = \varphi(\sum_i{w_i x_i} + b)
$$

Activation functions:



| Name        | Plot           | Function  | Derivative |
| ------------|----------------| --------- | ---------- |
| Sigmoid | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Activation_logistic.svg/120px-Activation_logistic.svg.png) | $$\frac{1}{1 + e^{-x}}$$ | $$f(x)(1 - f(x))$$ |
| Hyperbolic Tangent | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/c/cb/Activation_tanh.svg/120px-Activation_tanh.svg.png) | $$\frac{e - e^x}{e + e^x}$$ | $$1 - f(x)^2$$ |
| ReLU | ![](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fe/Activation_rectified_linear.svg/120px-Activation_rectified_linear.svg.png) | $$\begin{cases}
0 &\text{if} \ x \leq 0 \\
1 &\text{if} \ x > 0 \\
\end{cases}$$ | $$
\begin{cases}
0 &\text{if} \ x < 0 \\
1 &\text{if} \ x > 0 \\
undefined &\text{if} \ x = 0 
\end{cases}
$$ |
