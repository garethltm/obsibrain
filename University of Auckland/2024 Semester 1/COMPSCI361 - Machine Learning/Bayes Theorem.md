- everything is uncertain $\rightarrow$ everything is TRUE to a certain degree
	- finding more FALSE statements to disprove a hypothesis
- Search the most likely hypothesis 
	- giving the most likely model/proposition
$$P(Y|X) = \frac {P(X|Y)P(Y)}{P(X)}$$
which is short for $\forall \tiny{x,y}$: 
$$
P(Y=y | X=x) = \frac{P(X=x | Y=y) P(Y=y)}{P(X=x)}

$$
- big P = discrete random values
- small p = continuous random values (probability density)
## Basic assumption
- Quantities of interest are governed by probability distributions
- Optimal decisions can be made by reasoning about these probabilities together with observed [[training data]]

[[Machine Learning (ML)]] is interested in the best hypothesis h from space H, given observed [[training data]] D
best hypothesis $\approx$ most probable hypothesis
- highest probability given the [[training data]]
[[2024 Semester 1/COMPSCI361 - Machine Learning/Bayes Theorem|Bayes Theorem]] provides a direct method of calculating the probability of such a hypothesis based on:
- its prior probability
- the probabilities of observing various data given the hypothesis
- the observed data itself

