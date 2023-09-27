# Artificial Neural Network using Python and Numpy

In this project, we use python numpy library to create ANN models to perform:

- Addition with two inputs
- Multiplication with two inputs

## Theory 

An Artificial Neural Network consists of layers of artificial neurons. It is a collection of inputs, a set of weights, and output. These inputs are converted into a single output, which can then be used as an input for next layer of neurons. Each neuron has a weight vector where we have a number of inputs. These inputs can either be the raw input features or the output of neurons from the previous layer.

In an artificial neural network, we compute the weighted sum of all inputs in the input layer, and pass this sum through an activation function, also known as a nonlinear function. Activation functions can be of various types, like the Sigmoid Function, reLU, or Step function. This output can then be used in the next layer as input to that layer's neurons, and this process can be repeated for each layer in the network.

## Implementation

### Training Process

The training process consists of the following steps:

1. Forward Propagation: We take the two inputs from the input layer and multiply each input by the corresponding weight. Initially, random values of weights can be selected.
Let Y = WiIi = W1I1+W2I2+W3I3 
Pass the result through an activation function. For example, if we are using a sigmoid formula to calculate the neuron’s output, we normalize the result between 0 and 1: 
1/1 + e-y

2. Back Propagation: 
Calculate the error i.e the difference between the actual output and the expected output. Depending on the error, adjust the weights by multiplying the error with the input and again with the gradient of the Sigmoid curve: 
Weight += Error Input Output (1-Output) ,here Output (1-Output) is derivative of sigmoid curve.

3. Updating Parameters (Weights,Bias,Learning Rate):
The learning rate, weights, biases are updated according to the error function.The parameters are kept modifying until the error is minimum, and predicted and target value are the closest. Performance metrics can be used to evaluate the performance of the network.

### Evaluating the Model 

In order to evaluate the model, we use a Loss curve. The loss curve should show decreasing loss with time/epochs. A loss curve that does not decrease over time shows that your model may not be learning properly. 

## Conclusion 

We conclude that the activation functions and hidden layers bring non-linearity to the network and are suitable for common machine learning tasks like classification, regression and clustering. The addition and multiplication neural network models were implemented using python and numpy, without the use of any machine learning or deep learning frameworks, considering the relatively low amount of training data, the network performed considerably well in approximating both the operations. The loss v/s epochs curve was plotted to understand how the epochs increase with parameters and how the loss decreases gradually leading us closer to the target values.



