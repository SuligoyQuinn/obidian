# Subtraction
- Negate subtrahend and add
	- Assume all integers are same number of bits
	- ignore carry out
# Floating Point
- Large values $6.023\cdot 10^{23}$ require 79 bits
- Small values $6.626\cdot 10^{-34}$ require >110 bits
- 1 bit Sign, 8 bit exponents, 23 bit fraction
$$
N=(-1)^S\cdot 1.\text{fraction}\cdot 2^{\text{exponent-127}}, 1\leq \text{exponent}\leq 254
$$
$$
N=(-1)^S\cdot 0.\text{fraction}\cdot 2^{-126}, \text{exponent=0}
$$
