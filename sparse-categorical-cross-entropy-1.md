# 🟢 Sparse categorical cross entropy

* Use Case: Multi-class classification with integer labels (<mark style="color:purple;background-color:purple;">**no one-hot encoding**</mark>)
* Model Output: Probability distribution over classes (softmax)
* True Labels: Integer index of the correct class
* <mark style="color:purple;background-color:purple;">**We only look at the predicted probability for the true class.**</mark>
* <mark style="color:purple;background-color:purple;">**Loss = - log(p\_true)**</mark>
* p\_true = predicted probability of the correct class
* Batch Loss: Loss = (1/N) \* Σ (-log(p\_true\_i)) for i = 1 to N
* <mark style="color:purple;background-color:purple;">**Only the correct class contributes to the loss**</mark>
* Example Setup: Classes = 3, true class = 1, predicted p = \[0.05, 0.9, 0.05]
* Example Calculation: Loss = -log(0.9) ≈ 0.105
* Another Example (wrong prediction): Predicted p = \[0.8, 0.1, 0.1], true class = 1, Loss = -log(0.1) ≈ 2.302
* Quick Reference Table:

| True class (index) | Predicted p        | Loss Formula | Loss Value |
| ------------------ | ------------------ | ------------ | ---------- |
| 1                  | \[0.05, 0.9, 0.05] | -log(0.9)    | 0.105      |
| 1                  | \[0.8, 0.1, 0.1]   | -log(0.1)    | 2.302      |
| 0                  | \[0.7, 0.2, 0.1]   | -log(0.7)    | 0.357      |

* Key Points: Penalizes confident wrong predictions, memory-efficient, equivalent to categorical cross entropy but simpler for integer labels
