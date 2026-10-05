# Normal Distributions
## Standard Normal Distribution
- used to model many natural phenomena.
PDF:
$$
fz(z)=\frac{1}{\sqrt{ 2\pi }}e^{-z^2/2}
$$
Mean:
$$
E[Z]=0
$$
Variance:
$$
Var[Z]=1
$$
### Linear Functions of Standard Normal RVs
- Let $Z \sim N(0,1)$ be a standard normal random variable. For any constants $\mu$ and $\sigma$, the random variable $X=\sigma Z+\mu$ follows the normal distribution
$$
X\sim N(\mu,\sigma)
$$
### Standardizing Normal RVs
- If $X\sim N(\mu,\sigma)$ then $Z=\frac{X-\mu}{\sigma}$ follows the standard normal distribution:
$$
Z\sim N(0,1)
$$
## Normal Probabilities
- if $X$ is a normal random variable with mean $\mu$ and standard deviation $\sigma$ and $Z$ is a standard normal random variable, then
$$
P(X\leq x)=\phi\left( \frac{x-\mu}{\sigma} \right)
$$
## Normal Quantiles
- Let $X$ be a random variable and let $0\leq p\leq_{1}$ represent a quantile or percentile of $X$. The quantile function is a function that finds the value of x such that $P(X\leq x)=p$. For a normal variable, the quantile function is denoted as $\phi^-1(p)$.