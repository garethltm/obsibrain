- In [[Supervised Learning]]:
	- We have features $x_i$ & class labels $y_i$
	- Write a program that produces $y_i$ from $x_i$
- In [[Unsupervised Learning]]:
	- We only have $x_i$ values, but no explicit target labels (no targets)
	- You want to do "something" with them (potentially learning patterns)
		- learning some patterns from your data

#compsci345example - some [[Unsupervised Learning]] tasks:
1. Outlier detection
	- Is this a 'normal' $x_i$?
2. Similarity search
	- Which examples look like this $x_i$?
3. Association rules
	- Which $x_j$ occur together?
4. Latent-factors (what is the document mainly talking about - topics, [[Clustering]] based on topics)
	- What 'parts' are the $x_i$ made from?
5. Data visualization (used alot)
	- What does the high-dimensional X look like?
6. Ranking ([[Attribute (Feature) selection]])
	- Which are the most important $x_i$?
7. [[Clustering]] (what types of [[instance(s)]] are there?)
	- What types of $x_i$ are there?

## Summary
- fitting data without explicit labels