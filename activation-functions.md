---
hidden: true
---

# ⚔️ Activation Functions



| **Property**         | **Sigmoid**                                             | **Tanh**                                            | **ReLU**                                            | **Leaky ReLU**                                                 | **ELU**                                                     |
| -------------------- | ------------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | -------------------------------------------------------------- | ----------------------------------------------------------- |
| **Formula**          | $$\frac{1}{1 + e^{-x}}$$                                | $$\tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}$$    | $$\max(0, x)$$                                      | $$\begin{cases}x & x>0\\alpha x & x\le0\end{cases}$$           | $$\begin{cases}x & x>0\\alpha(e^x - 1) & x\le0\end{cases}$$ |
| **Output Range**     | (0, 1)                                                  | (-1, 1)                                             | \[0, ∞)                                             | (-∞, ∞)                                                        | (-α, ∞)                                                     |
| **Derivative**       | $$f(x)(1 - f(x))$$                                      | $$1 - f(x)^2$$                                      | $$\begin{cases}1 & x>0 & x\le0\end{cases}$$         | $$\begin{cases}1 & x>0\\alpha & x\le0\end{cases}$$             | $$\begin{cases}1 & x>0\f(x) + \alpha & x\le0\end{cases}$$   |
| **Derivative Range** | (0, 0.25)                                               | (0, 1)                                              | {0, 1}                                              | \[α, 1]                                                        | (0, 1+α)                                                    |
| **Pros**             | • Smooth and bounded• Interpretable as probability      | • Zero-centered• Stronger gradients than sigmoid    | • Fast and simple• Reduces vanishing gradient issue | • Solves dying ReLU partially• Allows small negative gradients | • Smooth• Reduces vanishing gradients• Zero-centered        |
| **Cons**             | • Vanishing gradient for large \|x\|• Not zero-centered | • Still suffers vanishing gradients for large \|x\| | • Dying ReLU problem• Not zero-centered             | • Choice of α is heuristic                                     | • More expensive computation                                |
