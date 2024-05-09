- document attributes are independent given the document class 
- #compsci361example probability of words in 1 text position are independent of the words occurring in the other positions given the document class (given a particular class)

$$
c_{MAP} = \arg \max_{c \in C}{P(x_1|c) P(x_2|c) \ldots P(x_n|c)}{P(c)}
$$

$$
= \arg \max_{c \in C} P(c) \prod_{i} P(x_i|c)
$$
- we need to estimate $n* |X|*|C|+|C|$ probability terms
- Even for simple use cases this is prohibitively large
	- #compsci361example  about 10 million terms for $|X| = 5000$, $|C|=2$, $n=100$ where $n$ is the length of text
- Since $P(x_i | v_k) = 1$ and $\sum_{x_i \in C} P(x_i | c_j) = 1$, we only need to estimate $\prod_{x_i \in V} P(x_i | c_j) = P(V_1 | c_1) \times \ldots \times P(V_n | c_1)$
