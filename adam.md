# 🔴 Adam

* <mark style="color:purple;background-color:purple;">**Combines the ideas of momentum and RMSProp.**</mark>
* <mark style="color:purple;background-color:purple;">**Adapts learning rates for each parameter individually.**</mark>
* <mark style="color:purple;background-color:purple;">**Includes bias correction for moving averages in early steps.**</mark>



1. **Compute exponential moving average of gradients (first moment, like momentum):**

* $$m_t = \beta_1 m_{t-1} + (1-\beta_1) g_t$$
* $$m_t$$ ≈ “momentum”
* $$\beta_1$$ = decay rate for first moment (usually 0.9)

2. **Compute exponential moving average of squared gradients (second moment, like RMSProp):**

* $$v_t = \beta_2 v_{t-1} + (1-\beta_2) g_t^2$$
* $$v_t$$ ≈ “RMS of gradients”
* $$\beta_2$$ = decay rate for second moment (usually 0.999)

3. **Bias correction** (especially important for early steps)

* $$\hat{m}_t = \frac{m_t}{1 - \beta_1^t}, \quad \hat{v}_t = \frac{v_t}{1 - \beta_2^t}$$

3. **Parameter update:**

* $$\theta_{t+1} = \theta_t - \frac{\alpha}{\sqrt{\hat{v}_t} + \epsilon} \hat{m}_t$$
* $$\alpha$$ = learning rate (usually 0.001)
* $$\epsilon$$ = small number to avoid division by zero



* **m\_t** (first moment) → keeps direction of past gradients (momentum)
* **v\_t** (second moment) → scales step size according to past gradient magnitude (like RMSProp)
* **Bias correction** → prevents moving averages from being too small at the beginning



* Adam = **Momentum + RMSProp + Bias correction**
* Automatically adapts **step size per parameter**
* Widely used in **deep learning** because it usually **converges faster and more reliably**

