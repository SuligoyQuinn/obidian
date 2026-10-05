# Random Variables, PMFs, PDFs, and CDFs
## Random Variable
- Random variable X corresponds to a random experiment. The value of the variable is not known until the experiment is performed. It is a function from the sample space S to a subset of the real numbers
- The probability that a random variable X equals the value x is denoted by
$$
P(X=x)
$$
### Discrete Random Variable
- one in which the possible outcomes are countable and is usually a subset of Z
### Continuous Random Variable
- one in which there are uncountably infinite outcomes and is usually a subset of R
## Probability Mass Function
- the PMF for a discrete random variable X is defined as
$$
P_{X}(x)=P(X=x)
$$
## Probability Density Function
- function such that the probability of the random variable X belonging to the interval (a,b) is computed as:
$$
P(a\leq X\leq b)=\int_{a}^b f_{X}(x)dx
$$
## Cumulative Distribution Function
- The CDF of a random variable X is defined as
$$
F_{X}(x)=P(X\leq x)
$$
For a discrete X this is
$$
F_{X}(x)=\sum_{k\leq x}P_{X}(k)

$$
For continuous X this is
$$
F_{X}(x)=\int ^x_{-\infty}f_{X}(t)dt
$$
- Shows probability that X is less than or equal to x