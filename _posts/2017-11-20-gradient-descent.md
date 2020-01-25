---
layout: post
title: 'What is gradient descent (for)?'
description: ""
categories: 
---

When normal equations are computationally expensive, such as with large feature
spaces, **linear regression may be solved using the Gradient Descent
algorithm**.

GD is a general optimization algorithm applicable to other methods as well,
such as neural networks.

Geometrically, gradient descent involves finding a minimum of a cost function
by taking small steps down the function towards a local minimum, such
that each step is taken in the direction of steepest descent
(the gradient).

Different initial values may be used to help find a global minimum when
multiple local minima exist.

The gradient of a function of n variables is a vector of n partial derivatives,
and is an extension of the concept of the derivative (1D functions).

Algebraically, gradient descent *simultaneously* updates the parameters
(thetas) iteratively:

	theta_j := theta_j - alpha*PD(J)
	
where:

	alpha =  the learning rate
	PD =  the partial derivative of the cost function J, w.r.t theta_j

Gradient descent is initialized with one or more random points, and iterations
proceed until convergence.

The best way to debug GD is by plotting the cost vs. the iteration. It should be
a decreasing curve. If not, then the learning rate is probably too high. On the
other hand, if the cost is not decreasing fast enough, the learning rate may be
increased.


# Appendix

The closed-form solution for linear regression, with `m` examples and `n`
features, is:

	beta_hat = inv(t(X)*X)*t(X)*y
	
where

	X is an (m x n+1) matrix (extra 1 for the intercept)
	y is a vector of length m
	beta_hat is a vector of length n+1
