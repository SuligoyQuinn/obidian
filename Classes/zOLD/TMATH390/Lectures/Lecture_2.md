# Data Types
- Non numerical data that only fits into a category is _qualitative_
- data measured on a numerical scale is _quantitative_
## Quantitative Data Types
- data is _discrete_ when there are finite or countably infinite number of distinct values
- data is _continuous_ when there are uncountably many values
# Measures of Central Tendency
## Mean
- mean of a dataset if the sum of the data divided by the number of entries
$$
\bar{x}=\frac{1}{n}\sum x_{i}
$$
- affected by outliers
## Median
- median of a dataset is the middle of the data when the dataset is ordered
- median is the $\frac{n+1}{2}$ value if n is odd or $\frac{\frac{n}{2}+\frac{n+2}{2}}{2}$ if n is even
## Mode
- the data value that occurs most frequently in the dataset
# Measures of Variance
## Quantiles and Percentiles
- _Quantiles_ are cut points the divide the data into equal parts that contain the same percentage of data
- _Percentiles_ are quantiles that divide the data into 100 equal parts.
- _Quartiles_ are quantiles that divide the data into 4 equal parts.
## Minimum and Maximum
- _Minimum_ is the smallest number in a data set
- _Maximum_ is the largest number in a data set
## Counts and Proportions
- _Count_ is the number of observations belonging to a certain category
- _Proportion_ is the number of observations belonging to a category divided by the total number of observations
## Range and IQR
- _Range_ is max divided by min
- _IQR_ or interquartile range is the difference between Q3 and Q1
## Five-Number Summary
- Describes data using the minimum, Q1, the median, Q3, and the maximum
## Outliers
- an _outlier_ is an observations that seems to be far away from the bult of the data
- a _low-outlier_ is any observation below $Q_{1}-1.5*IQR$
- a _high-outlier_ is any observation above $Q_{3}+1.5*IQR$
## Sample Variance and Standard Deviation
- an estimate of the population variance
$$
s^2=\frac{1}{n-1}\sum(x_{i}-\bar{x})^2
$$
- sample standard deviation
$$
s=\sqrt{ s^2 }
$$
## Summarizing
- can be used for central tendency qualitative data
	- Mode
	- Median
- can be used for variability of qualitative data
	- Counts
	- Proportions