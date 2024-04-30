- ***Learning is just another application of [[2024 Semester 1/COMPSCI361 - Machine Learning/Bayes Theorem|Bayes Theorem]]***

Given data set D, we want to find the best hypothesis h
- [[Bayesian Learning]] used $P(h|D)$, the [[conditional probability]] of a hypothesis given the data to define the "best"
$$P(h|D) = \frac{P(D|h)P(h)}{P(D)}$$
- Both $h$ and $D$ are events:
	- $D$: the event that we observed this particular data set
	- $h$: the event that the hypothesis h is the true hypothesis
	- Hypothesis $h$ and observed data set $D$ to substitute $X$ and $Y$ in [[2024 Semester 1/COMPSCI361 - Machine Learning/Bayes Theorem|Bayes Theorem]]![[Pasted image 20240429145259.png]]
## Why is it so important?
1. Explicit manipulation of probabilities - (it defines a class/paradigm for creating new algorithms)
	- Among the most practical approaches to certain types of learning problems
	- #compsci361example [[Bayes Optimal Classfier]] is competitive with [[Decision Tree(s)]] & ANN
2. Useful framework for understanding learning methods that do not explicitly manipulate probabilities - (it creates a framework to reason with all the other algorithms out there)
	- Determine conditions under which algorithms output the most probable hypothesis
	- #compsci361example justification of [[Least Squares]] error function, why smaller [[Decision Tree(s)]] are preferred (Occam's razor)
## Practical difficulties
1. Initial knowledge of many probabilities is required
	- In reality, might not have all knowledge $\rightarrow$ most likely unexpected
2. Significant computational costs required