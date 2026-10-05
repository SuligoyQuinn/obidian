# Maximum Likelihood Estimation
## Likelihood Function
- Let $X = X_{1},X_{2},\dots,X_{n}$ be a random sample of independent and identically distributed discrete random variables with PMF $P_{X}(x;\theta)$ where $\theta=(\theta_{1},\theta_{2},\dots,\theta_{n})$ is a vector of model parameters. The likelihood function is:
$$
L(\theta;x)=\prod^n_{i=1}P_{X}(x_{i};\theta)
$$
## Maximum Likelihood Estimation
- maximum likelihood estimator is value of parameter that maximizes the likelihood function
- given log-likelihood function $\ell(\theta;x)$ it is defined as:
$$
\hat{\theta}=\arg\max\ell(\theta;x)
$$
