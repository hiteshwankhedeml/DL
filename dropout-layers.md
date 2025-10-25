# 🟢 Dropout Layers

* Overfitting ⇒ Training accuracy = 90% , Testing accuracy = 60%
* We want to create a generalized model
* Since there are so many weights in ANN so it might also overfit
* We might remove some neurons from input and then in next layer also we might remove some neurons
* In next iteration, some other neurons might get deactivated
* <mark style="color:purple;background-color:purple;">**In test, all the neurons will be connected ⇒ there will be no dropout**</mark>
* <mark style="color:purple;background-color:purple;">**Suppose in 1st layer, we had used probability = 0.5 for removing neurons, then all the weights of thsi layer will be multiplied by 0.5 in test**</mark>
* No. of neurons to be deactivated is hyper parameter
