# 🟢 RMS Prop

* <mark style="color:purple;background-color:purple;">**In Adagrad, learning rate decreases too much over time because it sums all past squared gradients.**</mark>
* <mark style="color:purple;background-color:purple;">**Here,**</mark>**&#x20;**<mark style="color:red;background-color:purple;">**we use exponentially decaying average of squared gradients instead of a cumulative sum**</mark>
* <mark style="color:purple;background-color:purple;">**we give more weight to the accumulated gradient (past gradients), but still consider the current gradient**</mark>
* We are using exponential weighted average
* Here we are using beta value also for restricting
* Since we are squaring the derivative term, it can become very big also but we are restricting it using beta
* So here are using dynamic learning rate
* Also smoothing concept is also brough here, using exponential weight average&#x20;
*

    <figure><img src=".gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>
