# 🟢 Adagrad

* <mark style="color:purple;background-color:purple;">**Learning rate dynamic**</mark>
* So <mark style="color:purple;background-color:purple;">**initially for convergence it should take bigger steps and when it reaches minima, its speed should decrease**</mark>
* <mark style="color:purple;background-color:purple;">**Learning rate is different for each parameter**</mark>

***

#### Step 1: Setup

* Initial parameter: $$\theta_0 = 1.0$$
* Learning rate: $$\alpha = 0.1$$
* Small constant: $$\epsilon = 10^{-8}$$
* Gradients: $$g^{(1)} = 0.2, g^{(2)} = 0.4, g^{(3)} = 0.1$$

***

#### Step 2: Accumulate squared gradients

$$
G^{(t)} = \sum_{\tau=1}^{t} (g^{(\tau)})^2
$$

| Step | Gradient (g^{(t)}) | (G^{(t)})          |
| ---- | ------------------ | ------------------ |
| 1    | 0.2                | 0.2² = 0.04        |
| 2    | 0.4                | 0.04 + 0.16 = 0.20 |
| 3    | 0.1                | 0.20 + 0.01 = 0.21 |

***

#### Step 3: Compute effective learning rate

$$
\alpha_\text{eff}^{(t)} = \frac{\alpha}{\sqrt{G^{(t)} + \epsilon}}
$$

| Step | α\_eff | Calculation                        |
| ---- | ------ | ---------------------------------- |
| 1    | 0.5    | 0.1 / √(0.04 + 1e-8) ≈ 0.1 / 0.2   |
| 2    | 0.224  | 0.1 / √(0.20 + 1e-8) ≈ 0.1 / 0.447 |
| 3    | 0.218  | 0.1 / √(0.21 + 1e-8) ≈ 0.1 / 0.458 |

***

#### Step 4: Update θ

$$
\theta^{(t+1)} = \theta^{(t)} - \alpha_\text{eff}^{(t)} \cdot g^{(t)}
$$

| Step | θ\_prev | Δθ                   | θ\_new | Calculation     |
| ---- | ------- | -------------------- | ------ | --------------- |
| 1    | 1.0     | 0.5 × 0.2 = 0.1      | 0.9    | 1.0 - 0.1       |
| 2    | 0.9     | 0.224 × 0.4 ≈ 0.0896 | 0.8104 | 0.9 - 0.0896    |
| 3    | 0.8104  | 0.218 × 0.1 ≈ 0.0218 | 0.7886 | 0.8104 - 0.0218 |

***

**Observation:**

* The updates **get smaller over time** because Adagrad accumulates squared gradients in the denominator.
* This is how the learning rate adapts per step automatically.
* <mark style="color:$danger;background-color:red;">**In a very deep neural network, the alpha can be so big that learning rate will become very very small which might be approx to 0**</mark>
