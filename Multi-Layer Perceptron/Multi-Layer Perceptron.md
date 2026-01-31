# Artificial Neural Networks (ANN) 

ANN are the core building blocks of deep learning — simplified mathematical models inspired by biological neurons. Each artificial neuron takes multiple inputs, multiplies them by learnable weights, adds a bias, sums everything up (weighted sum), and passes the result through a non-linear activation function (like sigmoid, ReLU, tanh) to produce an output. When you stack many such layers, you get powerful pattern recognition capabilities.

## Multi-Layer Perceptron (MLP) 
MLP is the classic fully-connected feedforward ANN: input layer → one or more hidden layers → output layer. Every neuron in one layer connects to every neuron in the next (hence “fully connected”). MLPs are trained end-to-end using backpropagation + gradient descent — exactly what I was trying to understand by hand.

> Deep Learning builds on this idea but scales it massively: more layers, more neurons, more data, better automatic feature learning.
