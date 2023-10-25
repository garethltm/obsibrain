- $H(X,Y) = H(X) + H(Y|X)$
	- combination of [[Joint Entropy]] & [[Conditional Entropy]]
- $H(X\tiny 1\normalsize ,...,X\tiny n \normalsize) = H(X\tiny 1\normalsize) +H(X\tiny 2\normalsize | X\tiny 1\normalsize)+...+H(X\tiny n\normalsize |X\tiny 1\normalsize ,..., X\tiny n-1\normalsize)$
	- summation because of logs

#### Probability 
$$P(a \land b)=P(a)P(b\ |\ a)$$

### [[Bayesian Network Inference]]
![[COMPSCI3672023_S2W11Uncertainty2of2-16.jpg]]
Related to: [[conditional probability]]

> #Example 
> ![[COMPSCI3672023_S2W11Uncertainty2of2-17.jpg]]Related to: [[Local Markov Property]]
> ![[COMPSCI3672023_S2W11Uncertainty2of2-19.jpg]]Related to: [[Time Complexity]]
> Better method: [[Variable Elimination Algorithm (VE)]]