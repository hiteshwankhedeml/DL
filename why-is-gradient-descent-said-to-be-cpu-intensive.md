# 🟢 Why is gradient descent said to be cpu intensive

* Linear model with 4 weights: $$w_1, w_2, w_3, w_4$$
* Input vector: $$x = [x_1, x_2, x_3, x_4]$$
* Output: $$y_\text{pred} = w_1 x_1 + w_2 x_2 + w_3 x_3 + w_4 x_4$$
* Loss (MSE for one sample):\
  $$L = (y - y_\text{pred})^2$$
* Gradients:\
  $$\frac{\partial L}{\partial w_i} = -2 x_i (y - y_\text{pred}), \quad i=1,2,3,4$$
* CPU operations per weight per sample: 2 multiplications + 1 subtraction = 3 ops
* Total for 4 weights, 1 sample: $$(4 \times 3 = 12) ops$$
