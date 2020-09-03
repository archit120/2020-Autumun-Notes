### Books

1, Kevin Murphy: Machine Learning: A probabilistic Perspective - ideal



## Probabilistic Model

Given a set of observations $X$ we want $P(\theta | X) = g(X)$  where $\theta$ is model parameters



1. Inference $f_{\theta}(X) = P(Y|X, \theta)$ 

2. Model Comparison - 
   	1. $P(X|\theta_1) > P(X|\theta_2)$ 
    	2. $P(Y|X, \theta_1) > P(Y|X, \theta_2)$ 

  We are doing maximum likelihood modeling but we maximize likelihood of just $X$ or $X \cup Y$ or $Y|X$

$\theta = \max_\theta P(X(\theta))$