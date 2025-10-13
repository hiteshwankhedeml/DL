# 🟢 Relu

* Rectified linear unit
* <mark style="color:purple;background-color:purple;">**Output will be max of 0 or Z**</mark>
* <mark style="color:purple;background-color:purple;">**Derivative will be either 0 or 1**</mark>
* <mark style="color:purple;background-color:purple;">**If z is -ve its derivative will be 0, if its +ve then it will be 1**</mark>
* <mark style="color:purple;background-color:purple;">**If its 1 then weight updation will occur**</mark>
* <mark style="color:purple;background-color:purple;">**If its 0 then it creates a dead neuron**</mark>
*

    <figure><img src=".gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>
*

    <figure><img src=".gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>
*

    <figure><img src=".gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

<mark style="color:purple;background-color:purple;">**Pros:**</mark>

* <mark style="color:purple;background-color:purple;">**Solves vanishing gradient problem**</mark>
* <mark style="color:purple;background-color:purple;">**Calculations are fast**</mark>
* <mark style="color:purple;background-color:purple;">**Much faster than sigmoid or tanh**</mark>

<mark style="color:purple;background-color:purple;">**Cons:**</mark>

* <mark style="color:purple;background-color:purple;">**Dead neuron**</mark>
* <mark style="color:purple;background-color:purple;">**Not Zero centric**</mark>
