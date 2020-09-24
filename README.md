# Regularization-with-Keras
Regularization with Keras - MNIST Dataset

Regularization is a technique which makes slight modifications to the learning algorithm so that the model generalizes better. 
This in turn improves the model’s performance on the unseen data as well.

In machine learning, regularization penalizes the coefficients. In deep learning, it actually penalizes the weight matrices of the nodes.

Different Regularization Techniques in Deep Learning
Now that we have an understanding of how regularization helps in reducing overfitting, we’ll learn a few different techniques in order to apply regularization in deep learning.

L2 & L1 regularization
L1 and L2 are the most common types of regularization. These update the general cost function by adding another term known as the regularization term.

Cost function = Loss (say, binary cross entropy) + Regularization term

Due to the addition of this regularization term, the values of weight matrices decrease because it assumes that a neural network with smaller weight matrices leads to simpler models. Therefore, it will also reduce overfitting to quite an extent.

However, this regularization term differs in L1 and L2.

In L2, we have:



Here, lambda is the regularization parameter. It is the hyperparameter whose value is optimized for better results. L2 regularization is also known as weight decay as it forces the weights to decay towards zero (but not exactly zero).

In L1, we have:



In this, we penalize the absolute value of the weights. Unlike L2, the weights may be reduced to zero here. Hence, it is very useful when we are trying to compress our model. Otherwise, we usually prefer L2 over it.

