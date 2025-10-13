# 🔴 Vanishing Gradient Problem and Sigmoid

* This is 2 layered NN with sigmoid as activation function
*

    <figure><img src=".gitbook/assets/image (14) (1).png" alt=""><figcaption></figcaption></figure>

Sigmoid:

* It squeezes output between 0 and 1
* <mark style="color:purple;background-color:purple;">**If we want to update w1 then we will be using derivative and expand it using chain rule**</mark>
* <mark style="color:purple;background-color:purple;">**The output of sigmoid is between 0 and 1, and if we take its derivative then it will be 0 and 0.25**</mark>
* <mark style="color:purple;background-color:purple;">**Weights are also initialized smaller values between 0 and 1**</mark>
* <mark style="color:purple;background-color:purple;">**So a smaller value will be multiplied with weights**</mark>
* <mark style="color:purple;background-color:purple;">**So for w1, we will be multiplying so many smaller values, and it will be multiplied with small learning rate, so the change in w1 will be very very small**</mark>
* <mark style="color:purple;background-color:purple;">**If weights are not getting updated then we are not moving towards convergence**</mark>
* <mark style="color:purple;background-color:purple;">**This is known as vanishing gradient problem**</mark>
* <mark style="color:purple;background-color:purple;">**In a Deep NN, where we will be having more layers then we will be having this problem**</mark>
* To solve this researchers started exploring other activation function = tanh, relu, pre relu, swiss
*

    <figure><img src=".gitbook/assets/image (15) (1).png" alt=""><figcaption></figcaption></figure>
*

    <figure><img src=".gitbook/assets/image (16) (1).png" alt=""><figcaption></figcaption></figure>
