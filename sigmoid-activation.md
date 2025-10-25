# 🟢 Sigmoid Activation

* <mark style="color:purple;background-color:purple;">**Transforms value between 0 and 1**</mark>
* <mark style="color:purple;background-color:purple;">**Used in hidden layer**</mark>
*   <mark style="color:purple;background-color:purple;">**Derivative is in range of 0 and 0.25**</mark>

    <figure><img src=".gitbook/assets/image (17) (1).png" alt=""><figcaption></figcaption></figure>

<mark style="color:purple;background-color:purple;">**Cons:**</mark>

* When the input is away from the coordinate origin, the gradient of the function becomes very small, almost zero,  In backpropagation we use chain rule to calculate differentials of each weight w, so the differential of the chain is very small, which leads to <mark style="color:purple;background-color:purple;">**vanishing gradient problem**</mark>
* <mark style="color:purple;background-color:purple;">Slower</mark>
* <mark style="color:purple;background-color:purple;">**This is not zero centered function output (since its not passing through 0) - In ML we do standard scalar so it becomes 0 centered, so if data is 0 centered and function is also 0 centered then it will result in efficient weight update**</mark>

<mark style="color:purple;background-color:purple;">**Pros:**</mark>

* <mark style="color:purple;background-color:purple;">Smooth gradient, prevent jumps in output values</mark>
* <mark style="color:purple;background-color:purple;">Output between 0 and 1, normalizing the output of each neuron</mark>

