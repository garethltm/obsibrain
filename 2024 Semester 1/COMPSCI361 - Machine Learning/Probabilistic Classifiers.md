For years, best [[Spam Filtering]] methods used [[Naive Bayes]]

## [[Probabilistic Classifiers]] model the [[conditional probability]], $p(y\tiny {i}\normalsize|x\tiny {i}\normalsize)$
- "If a message has word $x\tiny {i}$, what is the [[Probability]] that the message is $spam$?"
- Classify it as spam if [[conditional probability]] of spam is higher than that of not spam
	- "If $p(y\tiny {i}\normalsize = 1|x\tiny {i}\normalsize) > p(y\tiny {i}\normalsize = 0|x\tiny {i}\normalsize)$" return "$spam$" else return "$not\ spam$"
