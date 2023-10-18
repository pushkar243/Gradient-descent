1: a) Write a code to implement the three versions of the gradient descent namely. vanilla gradient descent, mini batch gradient descent and stochastic gradient descent for a data set consisting of at least 1500 rows and 15 columns.

Implementation : This is implemented in the file** 1-Gradientdescent.ipynb**. To create the necessary dataset we have used python's random dataset generations. The objective of this problem statement was to learn gradient descent and implement it without using any of the deep learning models already available in python.

Observations/Brief theory: 
1.Vanilla gradient descent converes more smoothly than any other method.However it is more computationally intensive.
2.Stochastic gradient descent exhibits faster convergence however its more erratic. Its less computationally intensive.
3.Mini-Batch Gradient Descent: It strikes a balance between batch and stochastic gradient descent by using a small random subset (mini-batch) of the training data in each iteration and it introduces controlled noise.

b) In the 2nd part, implement mini batch method with batch size  of 16,32,64,128 and 256. Dataset is same as above.

Regarding mini batch method , there is always a trade off betweeen convergence and loss.Small batch size can introduce more noise but may lead to faster convergence while a large batch size can reduce noise but might converge more slowly.

**Please read the detailed theory in file : Theory for Gradient Descent and mini batch size.**

Observations: 
1.Best batch size for this data is 64.
2.We can see that convergence of data changes from batch size.

2 : Implement the line search methods (bisection, golden section and Armijo rule) on the data set taken for previous question. Lets write the observation.
Implementation: This is implemented in the file **2-linemethod.pynb**. 
Observations: In this example, Bisection works the best , then Armijio and last is Golden ratio. There is no one size fits all and it varies from one example to another.
Brief Theory : 
Bisection Line Search: Bisection iteratively divides an interval in half to find the local minimum, guaranteeing convergence but potentially requiring many iterations.
Golden Section Line Search: Golden Section Search uses the golden ratio to efficiently narrow down the interval containing the minimum, converging faster than simple bisection.
Armijo Rule Line Search: The Armijo Rule adaptively selects step sizes by comparing function values and a linear approximation, ensuring a sufficient reduction in the function value for optimization, often used in gradient-based algorithms.
**Please read the detailed theory in file : Theory for Line Search Method.**

3 : Given the function f(x) = (x^2 cos(x) + sin(x) − x), derive the variable step size (γ) that will ensure faster convergence of the gradient descent
method and compare the results
i) constant step size
ii) decaying step size using various values of α0 and k
iii) Bold driver algorithm

Implementation: This is implemented in the file **3-Gradientdescent-stepsize.pynb**. 
Observations : In this case , we can clearly see that bold driver's algorthim worked best.
Brief Theory: Certainly, here are one-liners for each of the three approaches:

Constant Step Size: Maintains a fixed step size (γ) throughout the optimization process, often chosen empirically.

Decaying Step Size: Adapts the step size by decreasing it over time ( γk= α0/(1+k) ), promoting faster convergence initially and stability later on.

Bold Driver Algorithm: Dynamically adjusts the step size using parameters α1 and α2, increasing the step size on improvement and decreasing it on performance degradation, enhancing convergence speed.
**Please read the detailed theory in file : Theory for Step Size in Gradient Descent Method.**
