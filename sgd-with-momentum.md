# 🟢 SGD with momentum

* <mark style="color:purple;background-color:purple;">**Using this we want to smoothen the curve so that noise is reduce and convergence happens fast**</mark>
* Below are the formula to update weights and bias
*   <mark style="color:purple;background-color:purple;">**Formula  can also be written as a time series**</mark>

    <figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
* <mark style="color:purple;background-color:purple;">**We can use exponential weighted average using this smoothening will happen**</mark>
* <mark style="color:purple;background-color:purple;">**Instead of updating weights directly with the current gradient, we use the velocity:**</mark>
* <mark style="color:purple;background-color:purple;">**w = w - learning\_rate \* v\_t**</mark>
* <mark style="color:purple;background-color:purple;">**The velocity accumulates past gradients, giving a “push” in directions where gradients are consistent**</mark>
* Lets say we have the below time and values
* If we join all the values in the plot, it wont be smooth
* Vt1 = a1
* Vt2 will be calculated using the new formula
* <mark style="color:purple;background-color:purple;">**Here we want previous value to control more, so we put β value more**</mark>
* This will smoothen the curve
*

    <figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
