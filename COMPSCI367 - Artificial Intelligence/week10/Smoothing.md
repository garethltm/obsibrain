- Applying [[Laplace smoothing (add-one smoothing)]] to our [[Language Model]] (Trigram)

$$\tilde{p}(\huge w\tiny 3\normalsize | \huge w\tiny 1\normalsize ,\huge w\tiny 2\normalsize) = \lambda \tiny 1 \ \normalsize \hat{p}(\huge w\tiny 3\normalsize | \huge w\tiny 1\normalsize ,\huge w\tiny 2\normalsize) + \lambda \tiny 2 \ \normalsize \hat{p}(\huge w\tiny 3\normalsize | \huge w\tiny 2\normalsize) +\lambda \tiny 3 \ \normalsize \hat{p}(\huge w\tiny 3\normalsize)\ + \in$$
- $\lambda \tiny 1 \ \normalsize \hat{p}(\huge w\tiny 3\normalsize | \huge w\tiny 1\normalsize ,\huge w\tiny 2\normalsize)$ for example doesn't work, there is still 
- $\lambda \tiny 1 \ \normalsize + \lambda \tiny 2 \ \normalsize +\lambda \tiny 3 \ \normalsize + \in \ =\ 1.0$
	- where $\in$ is like [[Laplace smoothing (add-one smoothing)]] (you use it if all has 0 possibilities)
