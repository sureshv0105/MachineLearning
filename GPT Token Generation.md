## Neural Network Components and Process

## 1. Neuron

A neuron is the basic computational unit in a neural network.

It takes inputs, applies weights and bias, processes the result through an activation function, and produces an output.

## 2. Weight

Each connection between neurons has a weight that determines the strength and importance of the input.

Every neuron in a layer receives multiple inputs from the previous layer, and each input is multiplied by a corresponding weight.

Weight and Edge Relationship: Weights are associated with the edges (connections) between neurons, not the neurons themselves. Each edge carries a unique weight that influences how much of the input is passed forward.

## 3. Bias

Each neuron has a unique bias value.

The bias is added to the weighted sum of the inputs before passing the result through the activation function. It helps the model shift the activation function to better fit the data.

## 4. Input Representation

Inputs to a neural network are represented as vectors or matrices.

For multiple tokens (e.g., in a language model), the input is a matrix where each row corresponds to an embedding vector of a token.

## 5. Processing in Layers

Each layer takes the input matrix and processes it through neurons.

Each neuron applies the following formula:


Here:

 + represents the inputs

 + represents the weights (specific to each incoming edge)

 + is the bias (unique to each neuron)

 + is the activation function

## 6. Output Representation

The final layer produces a single output vector representing a probability distribution over the entire vocabulary (in the case of language models).

Each value in this vector corresponds to the likelihood of a specific token being the next token.

## 7. Token Generation Process

For each step, the model:

Takes the input tokens and converts them into embeddings (a matrix).

Processes the embeddings through multiple layers.

Outputs a vector of probability distribution over the vocabulary (where the width of the vector equals the number of words in the vocabulary).

Selects the next token based on the probability distribution.

This process repeats token by token until the desired output is generated.
