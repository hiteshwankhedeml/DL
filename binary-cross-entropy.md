# 🟢 Binary cross entropy

* <mark style="color:purple;background-color:purple;">**We use log loss here ⇒  Same as used in logistic regression**</mark>
* Since this is binary classification problem, we use sigmoid in output layer
*   <mark style="color:purple;background-color:purple;">**Loss = - \[ y \* log(p) + (1 - y) \* log(1 - p) ]**</mark>

    <figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
*

    <table><thead><tr><th width="113.75">y</th><th width="104.5">p</th><th width="326.75">Loss Formula</th><th>Loss Value</th></tr></thead><tbody><tr><td>1</td><td>1</td><td>- [ 1 * log(1) + 0 * log(1 - 1) ]</td><td>0</td></tr><tr><td>1</td><td>0.9</td><td>- log(0.9)</td><td>0.105</td></tr><tr><td>1</td><td>0</td><td>- log(0)</td><td>∞</td></tr><tr><td>0</td><td>0</td><td>- [ 0 * log(0) + 1 * log(1 - 0) ]</td><td>0</td></tr><tr><td>0</td><td>0.1</td><td>- log(1 - 0.1)</td><td>0.105</td></tr><tr><td>0</td><td>1</td><td>- log(1 - 1)</td><td>∞</td></tr></tbody></table>
