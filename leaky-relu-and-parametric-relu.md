# 🟢 Leaky Relu and Parametric Relu

* <mark style="color:purple;background-color:purple;">**If we use alpha then its parametric relu, if we use constant value like 0.01 then its leaky relu**</mark>
* <mark style="color:purple;background-color:purple;">**Here even for -ve value we will get some output, so its derivative will also be not 0**</mark>
* <mark style="color:purple;background-color:purple;">**This solves dead relu issue**</mark>
*

    <figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Pros:

* Removes dead relu issue

Cons:

* Not Zero centric
