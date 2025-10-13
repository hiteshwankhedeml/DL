# 🟢 ANN Intuition and Learning

* Backward propagation was invented Geoffrey Hinton
* Dataset: IQ, Study hours, Play hours, Output
* Here we are having 2 layered NN
* Bias will also be added to each neuron
* In feed forward, we will assign weights and bias, which are assigned randomly
*

    <figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
* Forward Propagation:
* In 1st step we will do summation of x1w1 + x2w2 + x3w3 + b1, this will be our z
* After this we apply activation function on z
* O1 and O2 will be output of the neurons
* Difference between actual and predicted, will be error
* We have to reduce the error
* To minimize the error, we have to update the weights
* Once we have the error from the the 1st record, we will back propagate and then update the weights
* Similarly we will do for 2nd record and all
* <mark style="color:purple;background-color:purple;">**Cost function:**</mark> <mark style="color:purple;background-color:purple;"></mark><mark style="color:purple;background-color:purple;">If we calculate difference between actual and predicted then for all the points using summation</mark>
* <mark style="color:purple;background-color:purple;">**Error function:**</mark> <mark style="color:purple;background-color:purple;"></mark><mark style="color:purple;background-color:purple;">If we calculate difference for a single point</mark>
*

    <figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
*

    <figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
