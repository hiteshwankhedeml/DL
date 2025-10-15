# 🟢 Gradient Descent Optimizers

* Optimizer is responsible to reduce the loss in backward propagation
* <mark style="color:purple;background-color:purple;">**The formula for weight update will change for every optimizer**</mark>
*

    <figure><img src=".gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>
* If dataset has 1000 data points
* We calculate cost function for all the 1000 data points
* Using GD we will be doing gradient descent and weights will be updated
* <mark style="color:purple;background-color:purple;">**1 forward and 1 backward propagation is known as EPOCH**</mark>
* This will be repeated for all the EPOCH
*

    <figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>
* <mark style="color:purple;background-color:purple;">**In GD, 1 EPOCH = 1 iteration**</mark>
* <mark style="color:purple;background-color:purple;">**If we break into 10 iteration, then in 1st iteration we will pass 100 records and so on**</mark>
* <mark style="color:purple;background-color:purple;">**And this 10 iteration will form 1 EPOCH**</mark>
* But in GD we don't do this

**Advantage:**

* Convergence will happen

**Disadvantage:**

* <mark style="color:purple;background-color:purple;">**Huge resource ⇒  GPU, RAM ⇒  Resource intensive**</mark>

