# 🟢 Exponential weighted average

* <mark style="color:purple;background-color:purple;">**Smooths a sequence of values by giving more weight to recent values and less to older values**</mark>
* <mark style="color:purple;background-color:purple;">**Formula:**</mark> $$v_t = β * v_(t-1) + (1 - β) * x_t$$
  * <mark style="color:purple;background-color:purple;">**v\_t = current smoothed value**</mark>
  * <mark style="color:purple;background-color:purple;">**v\_(t-1) = previous smoothed value**</mark>
  * <mark style="color:purple;background-color:purple;">**x\_t = current value (e.g., gradient)**</mark>
  * <mark style="color:purple;background-color:purple;">**β = decay factor (0 < β < 1), typically 0.9**</mark>
* Intuition: Older values decay exponentially, recent values have higher influence
* Example Table:

| t | x\_t (current value) | v\_(t-1) (previous avg) | v\_t = β\*v\_(t-1)+(1-β)\*x\_t |
| - | -------------------- | ----------------------- | ------------------------------ |
| 1 | 0.5                  | 0                       | 0.05                           |
| 2 | 0.6                  | 0.05                    | 0.095                          |
| 3 | 0.4                  | 0.095                   | 0.0855                         |

* Application: Used in SGD with momentum to smooth gradients and accelerate convergence
