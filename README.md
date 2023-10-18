1: a) Write a code to implement the three versions of the gradient descent namely. vanilla gradient descent, mini batch gradient descent and stochastic gradient descent for a data set consisting of at least 1500 rows and 15 columns.

Implementation : This is implemented in the file 1-Gradientdescent.ipynb. To create the necessary dataset we have used python's random dataset generations. The objective of this problem statement was to learn gradient descent and implement it without using any of the deep learning models already available in python.

Observations: 
1.Vanilla gradient descent converes more smoothly than any other method.However it is more computationally intensive.
2.Stochastic gradient descent exhibits faster convergence however its more erratic. Its less computationally intensive.
3.Mini-Batch Gradient Descent: It strikes a balance between batch and stochastic gradient descent by using a small random subset (mini-batch) of the training data in each iteration and it introduces controlled noise.

b) In the 2nd part, implement mini batch method with batch size  of 16,32,64,128 and 256. Dataset is same as above.

Regarding mini batch method , there is always a trade off betweeen convergence and loss.Small batch size can introduce more noise but may lead to faster convergence while a large batch size can reduce noise but might converge more slowly.

Please read the detailed theory in file : Theory for Gradient Descent and mini batch size.

Observations: 
1.Best batch size for this data is 64.
2.We can see that convergence of data changes from batch size.

2 : Implement the line search methods (bisection, golden section and Armijo rule) on the data set taken for previous question. Lets write the observation.
Implementation: This is implemented in the file 2-linemethod.pynb. 
Observations: In this example, Bisection works the best , then Armijio and last is Golden ratio. There is no one size fits all and it varies from one example to another.

Please read the detailed theory in file : Theory for Line Search Method.

