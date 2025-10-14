# 🟢 Softmax for Multiclass Classification

* <mark style="color:purple;background-color:purple;">**For multi class classification, in output layer we use softmax activation function**</mark>
* <mark style="color:purple;background-color:purple;">**In binary classification, in output layer we have sigmoid activation as it transforms then value between 0 and 1**</mark>
* <mark style="color:purple;background-color:purple;">**Raw values from the previous layer (called logits) can be any real numbers — not restricted between 0 and 1.**</mark>
* <mark style="color:purple;background-color:purple;">**Classification problems usually need probabilities to:**</mark>
* <mark style="color:purple;background-color:purple;">**Interpret output easily (e.g., class with highest probability).**</mark>
* <mark style="color:purple;background-color:purple;">**Compare across classes meaningfully.**</mark>
* <mark style="color:purple;background-color:purple;">**Softmax converts logits into a probability distribution:**</mark>
* <mark style="color:purple;background-color:purple;">**All outputs are between 0 and 1.**</mark>
* <mark style="color:purple;background-color:purple;">**Sum of all outputs = 1.**</mark>
* <mark style="color:purple;background-color:purple;">**It also amplifies differences between logits — making the highest value more dominant, which helps in clear class prediction.**</mark>
*

    <figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>
*

    <figure><img src=".gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>
