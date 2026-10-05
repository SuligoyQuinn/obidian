# Discrete Distributions
## Bernoulli Random Variables
- models the outcomes of a binary experiment, when the probability of success is p
Mean:
$$
E[X]=\sum_{x=0}^1x*P_{X}(x)=0*(1-p)+1*p=p
$$
Variance:
$$
Var[X]=(0-p^2)*(1-p)+(1-p)^2*p=p(1-p)
$$
## Binomial Random Variable
- models the number of successful outcomes in a total of n trials where each trial has a probability of success p. Sum of n independent Bernoulli random variables
Mean:
$$
E[X]=np
$$
Variance:
$$
Var[X]=np(1-p)
$$
## Poisson Random Variable
- models the number of occurrences of an event when the events are independent and occur at a constant rate($\lambda$). This could be the number of occurrences in a given period of time or a given metric of space
Mean:
$$
E[X]=\lambda
$$
Variance:
$$
Var[X]=\lambda
$$
## Geometric Random Variable
- models the number of failures in a sequence of independent trials before a success occurs with the probability of success being p each time
Mean:
$$
E[X]=\frac{1-p}{p}
$$
Variance:
$$
Var[X]=\frac{1-p}{p^2}
$$
