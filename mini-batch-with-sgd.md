# 🟢 Mini Batch with SGD

* Since we have noise in SGD we use this
* Here we also use batch size
* <mark style="color:purple;background-color:purple;">**If we have 100k data points, then in EPOCH1**</mark>
* <mark style="color:purple;background-color:purple;">**Lets say batch size is 1000 records**</mark>
* <mark style="color:purple;background-color:purple;">**So in every iteration we take 1000 records and there will 100 iterations**</mark>
* For this 1000 data points we will find the cost function
* And using SGD optimizer we will update the weights
* This we will do for 100 iterations
* By brining the batch size we are reducing number of iterations as well as noise
*

    <figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

**Advantage:**

* <mark style="color:purple;background-color:purple;">**Better convergence speed compared to SGD**</mark>
* <mark style="color:purple;background-color:purple;">**Noise will be less when compared to SGD**</mark>
* <mark style="color:purple;background-color:purple;">**Efficient resource usage**</mark>

**Disadvantage:**

* <mark style="color:purple;background-color:purple;">**Noise still exists**</mark>
