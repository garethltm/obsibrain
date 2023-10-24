### estimating the [[probability]] of the whakatauki, "he waka eke noa"

$W = he\ waka\ eke\ noa$
$p(W) = ?$

- Trigram model (n-gram model for n = 3):
	- $p(W) \cong p(he)\cdot p(waka\ |\ he)\cdot p(eke\ |\ he,waka)\cdot p(noa\ |\ waka,eke)$
- Unigram model: $$p(\huge w\tiny 1\normalsize) = \frac {f(\huge w\tiny 1\normalsize)}{N}$$
- Bigram model: $$p(\huge w\tiny 2\normalsize | \huge w\tiny 1\normalsize) = \frac {f(\huge w\tiny 1\normalsize , \huge w\tiny 2\normalsize)}{f(\huge w\tiny 1\normalsize)}$$
	- where 