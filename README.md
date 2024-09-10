# NewScrach_Neural-Network

## Activation Functions

The following activation functions are implemented:

- **ReLU**: Rectified Linear Unit, used in hidden layers.
- **Tanh**: Hyperbolic tangent activation function, an alternative to ReLU.
- **Sigmoid**: Used in the output layer for binary classification.
- **Softmax**: Used for multi-class classification if needed.

## Cost Function

The cost function for binary classification is computed using the cross-entropy loss:

\[
\text{Cost} = -\frac{1}{m} \sum_{i=1}^{m} \left[ Y^{(i)} \log(A^{(i)}) + \left(1 - Y^{(i)}\right) \log\left(1 - A^{(i)}\right) \right]
\]

Where:
- \( m \) is the number of training examples.
- \( Y \) is the actual label.
- \( A \) is the predicted output.

## Forward and Backward Propagation

### Forward Propagation

- Data flows forward through the network, starting from the input layer, passing through all hidden layers, and ending at the output layer.
- The activation function (ReLU or Tanh) is applied after each hidden layer.
- In the final layer, the sigmoid function is applied for binary classification.

### Backward Propagation

- Gradients are computed using the chain rule to calculate the partial derivatives of the cost function with respect to the parameters.
- The parameters are updated using gradient descent.

## Training the Model

The training loop consists of the following steps:

1. **Initialize** the weights and biases.
2. **Perform forward propagation** to compute predictions.
3. **Calculate** the cost function.
4. **Perform backward propagation** to compute gradients.
5. **Update parameters** using gradient descent.
6. **Repeat** for a specified number of iterations.

## Results

The model is trained for a fixed number of iterations, and the training/testing accuracy and cost function are logged at intervals.

Example training results:

