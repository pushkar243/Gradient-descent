1: Write a code to implement the three versions of the gradient descent namely. vanilla gradient descent, mini batch gradient descent and stochastic gradient descent for a data set consisting of at least 1500 rows and 15 columns.

Write the necessary theory and experiment on the convergence using the optimal batch size for the mini batch method.

Implementation : This is implemented in the file 1-Gradientdescent.ipynb. To create the necessary dataset we have used python's random dataset generations. The objective of this problem statement was to learn gradient descent and implement it without using any of the deep learning models already available in python.

In the 2nd part, implemented mini batch method with batch size  of 16,32,64,128 and 256. Dataset is same as above.

Observations: 
1.Vanilla gradient descent converes more smoothly than any other method.However it is more computationally intensive.
2.Stochastic gradient descent exhibits faster convergence however its more erratic. Its less computationally intensive.
3.Mini-Batch Gradient Descent: It strikes a balance between batch and stochastic gradient descent by using a small random subset (mini-batch) of the training data in each iteration and it introduces controlled noise.


Regarding mini batch method , there is always a trade off betweeen convergence and loss.Small batch size can introduce more noise but may lead to faster convergence while a large batch size can reduce noise but might converge more slowly.


Observations: 
1.Best batch size for this data is 64.
2.We can see that convergence of data changes from batch size.




