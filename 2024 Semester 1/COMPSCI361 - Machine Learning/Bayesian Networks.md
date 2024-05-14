- [[Bayesian Belief Networks]] allow [[conditionally independent]] among subsets of variables
- Allows combining prior knowledge about (in)dependencies among variables with observed [[training data]]
	- We do not assume that everything is independent $\rightarrow$ there are more complicated relationships
		- some will be independent & some will be [[conditionally independent]]
## Motivation
- [[Naive Bayes]] assumption of [[conditionally independent]] is too restrictive
	- because they assume that a word appearing in 1 position of a text is completely unrelated to the word that appears in a different position
		- some structure is needed in order for a word to make sense in English
- but it's intractable without such assumptions