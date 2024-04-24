- reduce dimensionality by removing set of attributes (not transforming our input space into another space/operating in the original space - keep certain features only):
	1. [[Redundant attributes]]
	2. [[Irrelevant attributes]]
## Methods
1. [[Filters]]
2. [[Wrappers]]
- difference is how you see [[Attribute (Feature) Selection]] task as separate/combined from the learning task
## [[Attribute (Feature) Selection]] using Correlation
1. For nominal data:
	- given 2 attributes A & B with values $a\tiny {1}\normalsize ,...,a\tiny {c}$ &  $b\tiny {1}\normalsize ,...,b\tiny {r}$ the correlation can be calculated using the [[chi-squared test]] ($\chi ^2$) test