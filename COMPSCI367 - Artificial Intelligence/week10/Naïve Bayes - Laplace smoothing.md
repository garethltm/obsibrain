- [[Zipf's law]]
- bottom line is that some words are very rare & may not appear in a sample or will be undersampled, which leads to [[overfitting]]
- [[Laplace smoothing (add-one smoothing)]]

Given a vocabulary v of size d 
- of terms $\large v\tiny i$ for $i=(1,...,d)$
- counts $\large c\tiny i$ (counts for each of the terms) summing to N (total number of words)
we use a smoothed estimate of the [[probability]]:
$$\hat{P}(\large v\tiny i\normalsize)=\frac {\large c\tiny i\ \normalsize +\ \alpha}{N\ +\ \alpha d}=\frac {\large c\tiny i\ \normalsize +\ 1}{N\ +\ d}(for\ add-one\ case)$$
- for the case of [[Laplace smoothing (add-one smoothing)]]
	- we add 1 to each term of the count

![[Pasted image 20231025003904.png]]
