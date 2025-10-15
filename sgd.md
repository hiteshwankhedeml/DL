# 🟢 SGD

* <mark style="color:purple;background-color:purple;">**We pass single record in each iteration**</mark>
* <mark style="color:purple;background-color:purple;">**We calculate loss function, and then do backward propagation**</mark>
*

    <figure><img src=".gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

**Advantage:**

* <mark style="color:purple;background-color:purple;">**Solves resource issue**</mark>

**Disadvantage:**

* Time complexity increases
* <mark style="color:purple;background-color:purple;">**Convergence takes time**</mark>
* <mark style="color:purple;background-color:purple;">**Noise gets introduced ⇒  Since we are updating the weights based on a single record so it wont be a smooth convergence**</mark>
*

    <figure><img src=".gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>
