>	#Example 
>	estimating the [[probability]] of the whakatauki, "he waka eke noa"
>	$W = he\ waka\ eke\ noa$
>	$p(W) = ?$

- Trigram model (n-gram model for n = 3):
	- $p(W) \cong p(he)\cdot p(waka\ |\ he)\cdot p(eke\ |\ he,waka)\cdot p(noa\ |\ waka,eke)$


### Models
- Unigram model: $$p(\huge w\tiny 1\normalsize) = \frac {f(\huge w\tiny 1\normalsize)}{N}$$
- Bigram model: $$p(\huge w\tiny 2\normalsize | \huge w\tiny 1\normalsize) = \frac {f(\huge w\tiny 1\normalsize , \huge w\tiny 2\normalsize)}{f(\huge w\tiny 1\normalsize)}$$
	- where $f(\huge w\tiny 1\normalsize ,\huge w\tiny 2\normalsize)$ is the count of times $\huge w\tiny 2\normalsize$  follows $\huge w\tiny 1\normalsize$
	-
- Trigram model: $$p(\huge w\tiny 3\normalsize | \huge w\tiny 1\normalsize ,\huge w\tiny 2\normalsize) = \frac {f(\huge w\tiny 1\normalsize , \huge w\tiny 2\normalsize ,\huge w\tiny 3\normalsize)}{f(\huge w\tiny 1\normalsize , \huge w\tiny 2\normalsize)}$$
