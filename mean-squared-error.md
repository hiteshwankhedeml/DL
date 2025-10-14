# 🟢 Mean Squared Error

* <mark style="color:purple;background-color:purple;">**This loss function is in the form of quadratic equation**</mark>
* <mark style="color:purple;background-color:purple;">**If we plot this loss vs weights then it will have only 1 global minima**</mark>
*   This curve is known as gradient descent

    <figure><img src=".gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

<mark style="color:purple;background-color:purple;">**Advantage:**</mark>

* <mark style="color:purple;background-color:purple;">MSE is differentiable</mark>
* <mark style="color:purple;background-color:purple;">It has 1 local or global minima</mark>
* <mark style="color:purple;background-color:purple;">It converges faster ⇒  coz we have smooth gradient descent</mark>

<mark style="color:purple;background-color:purple;">**Disadvantage:**</mark>

* <mark style="color:purple;background-color:purple;">Not robust to outliers ⇒  As we are squaring so becoz of this cost function will increase ⇒  We are penalizing the cost function ⇒  becoz of this our best fit line will get shifted</mark>
