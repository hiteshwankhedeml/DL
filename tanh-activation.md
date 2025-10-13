# 🟢 Tanh Activation

* <mark style="color:purple;background-color:purple;">**Transforms value between -1 and +1**</mark>
* <mark style="color:purple;background-color:purple;">**Derivative ranges between 0 to 1**</mark>
* It is a hyperbolic tangent function
* <mark style="color:purple;background-color:purple;">**Zero centered**</mark>
* <mark style="color:purple;background-color:purple;">**For a medium sized NN it wont face any problem, but for very deep neural network we might still face vanishing gradient problem**</mark>
* In binary classification, tanh is used in hidden layer and sigmoid is used in output layer
*

    <figure><img src=".gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

**Cons:**

* Vanishing gradient exists for deep NN
* <mark style="color:purple;background-color:purple;">Computations are more</mark>

**Pros:**

* <mark style="color:purple;background-color:purple;">Zero centered ⇒ Weight updation efficient</mark>
