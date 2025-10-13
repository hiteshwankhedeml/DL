# 🟢 Perceptron Intuition

* It is a simple neural network unit
* We also call it as single layered NN
* <mark style="color:purple;background-color:purple;">**Perceptron is a basic unit of ANN**</mark>
* <mark style="color:purple;background-color:purple;">**Used in solving binary classifier**</mark>
* Dataset: Input: IQ, No. of study hours. Output: Pass/Fail
* We need to train weights&#x20;
* Inside a neuron 2 process happen:&#x20;
* <mark style="color:purple;background-color:purple;">**Step 1: Summation of weights and inputs + bias**</mark>
* <mark style="color:purple;background-color:purple;">**Step 2: Apply activation function**</mark>
* Weights are initially randomly processed, if all weights are 0 and there is no bias then there will be no output of neuron, so we add bias as noise
* <mark style="color:purple;background-color:purple;">**Activation function is to transform the output between some values(0 to 1, -1 to +1)**</mark>
*

    <figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>
*

    <figure><img src=".gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>
* <mark style="color:purple;background-color:purple;">**In step function, threshold will be 0**</mark>
* <mark style="color:purple;background-color:purple;">**In sigmoid function, threshold will be 0.5**</mark>
* For linear classification, with the help of perceptron we are able to create a line which can separate  classes
* That means perceptron is a linear classifier
