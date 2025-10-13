# Regression Cost Function

1. Mean Squared Error:

* This loss function is in the form of quadratic equation
* If we plot this loss vs weights then it will have only 1 global minima
*   This curve is known as gradient descent

    <figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Advantage:

* MSE is differentiable
* It has 1 local or global minima
* It converges faster -> coz we have smooth gradient descent

Disadvantage:

* Not robust to outliers -> As we are squaring so becoz of this cost function will increase -> We are penalizing the cost function -> becoz of this our best fit line will get shifted



2. **Mean Absolute Error:**

* if dataset has outlier then we use should use MAE
*   We use sub gradient here to calculate slope

    <figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

3. **Huber Loss:**

* Combination of MSE and MAE
*   If error below hyper-parameter then use MSE else MAE

    <figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

4. **RMSE:**

*

    <figure><img src=".gitbook/assets/image (9).png" alt="" width="375"><figcaption></figcaption></figure>
