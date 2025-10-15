# 🟢 Categorical Cross Entropy

* <mark style="color:purple;background-color:purple;">**Multi-class classification (more than 2 classes)**</mark>
* <mark style="color:purple;background-color:purple;">**Softmax is used in model output**</mark>
* Model Output: Probability distribution over classes (softmax)
* True Labels: One-hot encoded vector
* <mark style="color:purple;background-color:purple;">**- Σ ( y\_i \* log(p\_i) )**</mark>
* y\_i = 0 or 1 (true label for class i)
* p\_i = predicted probability for class i
* Only the correct class (y\_i = 1) contributes to loss
* Example: Classes = 3, true class = 2 → y = \[0,1,0], predicted p = \[0.05,0.9,0.05], Loss = -log(0.9) ≈ 0.105
* Example (wrong prediction): predicted p = \[0.8,0.1,0.1], true class = 2, Loss = -log(0.1) ≈ 2.302
* Quick Reference Table:
  *

      | True y (one-hot) | Predicted p        | Loss Formula | Loss Value |
      | ---------------- | ------------------ | ------------ | ---------- |
      | \[0, 1, 0]       | \[0.05, 0.9, 0.05] | -log(0.9)    | 0.105      |
      | \[0, 1, 0]       | \[0.8, 0.1, 0.1]   | -log(0.1)    | 2.302      |
      | \[1, 0, 0]       | \[0.7, 0.2, 0.1]   | -log(0.7)    | 0.357      |
* Key Points: Penalizes confident wrong predictions heavily, works with softmax output layer, equivalent to BCE when classes = 2
