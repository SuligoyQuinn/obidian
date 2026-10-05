# Continuous Distributions
## Uniform Random Variable
- given a range where a random variable can be any one of the values
- all positions are equally likely
- a lower bound, b upper bound
Mean:
$$
E[X]=\frac{a+b}{2}
$$
Variance:
$$
Var[X]=\frac{(b-a)^2}{12}
$$
## Exponential Random Variable
- models the time that passes before an event of interest occurs
PDF:
$$
fx(x;\lambda)=\lambda e^{-\lambda x}
$$
Mean:
$$
E[X]=\frac{1}{\lambda}

$$
Variance:
$$
Var[X]=\frac{1}{\lambda^2}
$$
## Gamma Random Variable
- models the total amount of time that passes before a certain number of events occur where the time between each event is exponentially distributed
- alpha is number of events
PDF:
$$
fx(x;\alpha,\lambda)=\frac{\lambda ^\alpha}{\gamma(\alpha)}x^{\alpha-1}e^{-\lambda x}
$$
Mean:
$$
E[X]=\frac{\alpha}{\lambda}
$$
Variance:
$$
Var[X]=\frac{\alpha}{\lambda^2}
$$
## Beta Random Variable
- models proportions. If Y is gamma random variable with shape alpha and rate lambda and Z is a random variable with shape beta and rate lambda. Then $X=\frac{Y}{Y+Z}$ is a beta random variable
PDF:
$$
fx(x;\alpha;\beta)=\frac{\gamma(\alpha+\beta)}{\gamma(\alpha)\gamma(\beta)}x^{\alpha-1}(1-x)^{\beta-1}

$$
Mean:
$$
E[X]=\frac{\alpha}{\alpha+\beta}

$$
Variance:
$$
Var[X]=\frac{\alpha \beta}{(\alpha+\beta)^2(\alpha+\beta+1)}
$$
