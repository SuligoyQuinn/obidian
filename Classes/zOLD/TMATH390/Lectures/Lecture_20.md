# Confidence Interval
- A confidence interval is a random interval that is designed in such a way that it is expected to contain a population parameter a certain percentage of the time. For a one dimensional parameter $\theta$, it is an interval with random bounds $L(\mathbf{X})$ and $U(\mathbf{X})$ such that:
$$
P(L(\mathbf{X})\leq \mu\leq U(\mathbf{X}))=1-\alpha
$$
- $1-\alpha$ is confidence level of the confidence interval
## CI for population mean given deviation
- Let $X_{1},X_{2},\dots,X_{n}$ be independent and identically distributed normal random variables with unknown mean $\mu$ and known standard deviation $\sigma$:
$$
\bar{X}\pm Z_{1-\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}
$$
## CI for population mean unknown deviation
$$
\bar{X}\pm t_{n-1,1-\frac{\alpha}{2}}\frac{S}{\sqrt{ n }}
$$
