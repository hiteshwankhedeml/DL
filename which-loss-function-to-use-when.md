# 🟢 Which Loss function to use when

| Hidden Layers       | Output Layer | Problem Statement          | Loss Function              |
| ------------------- | ------------ | -------------------------- | -------------------------- |
| Relu or its variant | Sigmoid      | Binary classification      | Binary cross entropy       |
| Relu or its variant | Softmax      | Multi class classification | Categorical or Sparse CE   |
| Relu or its variant | Linear       | Regression                 | MSE, MAE, Huber loss, RMSE |

| **Scenario**                                                                                                          | **Label Format Example** | **Loss Function**                     | **Why**                                                                                            |
| --------------------------------------------------------------------------------------------------------------------- | ------------------------ | ------------------------------------- | -------------------------------------------------------------------------------------------------- |
| <mark style="color:purple;background-color:purple;">**Multi-class classification with one-hot encoded labels**</mark> | `[0, 1, 0]`              | **categorical\_crossentropy**         | Expects one-hot vectors to find probability of the correct class                                   |
| <mark style="color:purple;background-color:purple;">**Multi-class classification with integer labels**</mark>         | `1`                      | **sparse\_categorical\_crossentropy** | Expects class index instead of vector                                                              |
| Binary classification (two classes, output 1 neuron with sigmoid)                                                     | `0` or `1`               | **binary\_crossentropy**              | For two-class problems, not multi-class                                                            |
| Multi-label classification (multiple independent 0/1 outputs)                                                         | `[1, 0, 1, 0]`           | **binary\_crossentropy**              | <mark style="color:purple;background-color:purple;">**Each class is treated independently**</mark> |
