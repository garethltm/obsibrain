- attributes are identically distributed given the document class
- #compsci361example the probability of seeing a specific word w is independent of the specific word position in the document, that is$$P(x_i = w|c) = P(x_j = w|c)$$ for $$1 \leq i \neq j \leq n$$ [[Independent & Identically Distributed (IID)]]
- We can use the same [[training data]] set to get more reliable estimates, because we need to estimate only $|X| \cdot |C| +|C|$ [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Probability|Probability]] terms. (position is out of the picture)
- [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Probability|Probability]] estimates are based on word counts in the [[training data]] set$$P(x_i = w|c) = \frac{\text{count}(w, c)}{\sum_{x \in X} \text{count}(x, c)}$$

- **$P(x_i = w|c)$**: Probability of each position we have our particular word.
- **$\text{count}(w, c)$**: Number of times the word occurs across all documents labeled ($c$).
	- (How many times this word appears)
- **$\sum_{x \in X} \text{count}(x, c)$**: Effectively the total length of all documents labeled ($c$)
