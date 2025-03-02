
## Neural Network
In a neural network, we have multiple layers. Each layer has a number of neurons. Each connection between neurons has a weight attached to it, and each neuron has an activation function. The role of a neuron is to take inputs, process them using these weights, and produce an output. This way, the neural network collectively learns patterns from the data. As the input is passed through each layer, the network captures simple patterns in the early layers and more complex patterns in deeper layers, and finally, an output is generated.

The output is compared to a ground truth, and a loss function quantifies the error. To reduce the error, we need to adjust the weights. This is where backpropagation comes in—the error signals propagate backward from the final layer to the first layer. 

The process has two main steps:
+ Forward Pass → Computes activations (left to right).
+ Backward Pass → Adjusts weights using gradients (right to left).

During backpropagation, we compute the gradient of the loss function with respect to each weight, which tells us how much each weight contributes to the error. Then, we update the weights to reduce the error and repeat the process.

Training typically stops when the model reaches an acceptable level of loss, when the gradient becomes very small (indicating minimal further improvement), or when performance on a validation set stops improving (early stopping). At this point, we can declare the model is trained.
