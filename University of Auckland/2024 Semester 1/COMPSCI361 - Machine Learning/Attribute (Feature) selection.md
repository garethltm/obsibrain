- reduce dimensionality by removing set of attributes (not transforming our input space into another space/operating in the original space - keep certain features only):
	1. [[Redundant attributes]]
	2. [[Irrelevant attributes]]
## Methods
1. [[Filters]]
2. [[Wrappers]]
- difference is how you see [[Attribute (Feature) selection]] task as separate/combined from the learning task
## [[Attribute (Feature) selection]] using Correlation
1. For nominal data:
	- given 2 attributes A & B with values $a\tiny {1}\normalsize ,...,a\tiny {c}$ &  $b\tiny {1}\normalsize ,...,b\tiny {r}$ the correlation can be calculated using the [[chi-squared test]] ($\chi ^2$) test (for categorical/numerical features)
	- We want to filter the features that are correlated with each other - Pairwise-comparison
2. For numerical data:
	- can be compared using [[Pearson's correlation coefficient]]
#### So what does correlation measure?

![[Pasted image 20240425014235.png]]
- Don't remove if 0 because it is calculating "linearly" 
	- if it is non-linear, you can divide your space & find multiple linear models (piecewise linear)
- How can it be used to remove redundant (input) or unimportant attributes (target variable)? - Pairwise