- [[Bayesian Belief Networks]] allow [[conditionally independent]] among subsets of variables
- Allows combining prior knowledge about (in)dependencies among variables with observed [[training data]]
	- We do not assume that everything is independent $\rightarrow$ there are more complicated relationships
		- some will be independent & some will be [[conditionally independent]]
## Motivation
- [[Naive Bayes]] assumption of [[conditionally independent]] is too restrictive
	- because they assume that a word appearing in 1 position of a text is completely unrelated to the word that appears in a different position
		- some structure is needed in order for a word to make sense in English
- but it's intractable without such assumptions
## Application
1. [[Naive Bayes Classifier]] is actually a special case of [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Bayesian Networks|Bayesian Networks]]
	- Variables: 
		- features $X_i$
		- class $Y_i$
	- Graph structure:![[Pasted image 20240515161532.png]]
2. [[Hidden Markov Model]]
## Inference
- How can one infer the (probabilities of) values of 1 or more network variables, given observed values of others?
- [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Bayesian Networks|Bayesian Networks]] contain all information needed for this [[inference(s)]]
- If only one variable with unknown value ( #compsci361example target in classification ), easy to infer it
	- #compsci361example [[Maximum A Posteriori (MAP) Hypothesis]]
	- If something isn't observed, we can use the [[Hidden Markov Model]] concept (structured in provided)
- In general case, the exact [[inference(s)]] is [[NP]]-hard ( #compsci361example a random approach is used - [[uninformed random walk]] ), approximations have been introduced ( #compsci361example Monte Carlo-based methods & variational [[inference(s)]]) - you find something similar & optimise
- In cases, the structure will need to be learned from the [[training data]] as well
	- typically using [[heuristic(s)]]
## Summary
- [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Bayesian Networks|Bayesian Networks]] provide a natural representation of [[conditionally independent]]
- Special case of [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Bayesian Networks|Bayesian Networks]] where we think everything becomes independent once we know the class