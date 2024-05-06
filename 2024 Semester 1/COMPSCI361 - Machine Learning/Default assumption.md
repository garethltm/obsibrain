- document attributes are independent given the document class 
- #compsci361example probability of words in 1 text position are independent of the words occurring in the other positions given the document class (given a particular class)

$$
c_{MAP} = \arg \max_{c \in C}{P(x_1|c) P(x_2|c) \ldots P(x_n|c)}{P(c)}
$$

$$
= \arg \max_{c \in C} P(c) \prod_{i} P(x_i|c)
$$
- we need to estimate $n* |X|*|C|+|C|$ probability terms
- Even for simple use cases this is prohibitively large, #compsci361example  about 10 million terms for |X| = 5000