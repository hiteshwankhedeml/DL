# 🟢 Adadelta

* <mark style="color:purple;background-color:purple;">**The numerator is the RMS (root mean square) of past parameter updates.**</mark>
* <mark style="color:red;background-color:purple;">**It controls the size of the step we take for this parameter.**</mark>
* <mark style="color:purple;background-color:purple;">**if past updates were small, the step stays small; if past updates were large, the step can be larger.**</mark>
* <mark style="color:purple;background-color:purple;">**Unlike RMSProp (where numerator is fixed α), Adadelta’s numerator adapts automatically based on history.**</mark>

#### **1. Moving average of squared gradients**

* $$E[g^2]t = \beta , E[g^2]{t-1} + (1-\beta) , g_t^2$$
* $$\beta$$ = decay rate (e.g., 0.9)
* $$g_t$$ = current gradient

***

#### **2. Parameter update (Δθ)**

* $$\Delta \theta_t = - \frac{\sqrt{E[\Delta \theta^2]_{t-1} + \epsilon}}{\sqrt{E[g^2]_t + \epsilon}} , g_t$$
* Numerator = RMS of past updates $$E[\Delta \theta^2]_{t-1}$$
* Denominator = RMS of current gradients $$E[g^2]_t$$
* $$\epsilon$$ = small constant to avoid division by zero

***

#### **3. Update parameter**

* $$\theta_{t+1} = \theta_t + \Delta \theta_t$$

***

#### **4. Update moving average of squared updates**

* $$E[\Delta \theta^2]t = \beta , E[\Delta \theta^2]{t-1} + (1-\beta) , (\Delta \theta_t)^2$$

***

* **Key point:** The numerator adapts automatically using past updates; no manual learning rate is needed.
