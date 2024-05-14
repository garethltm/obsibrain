- a probabilistic [[classifier(s)]] based on [[Bayes rule]]
- it tends to work well with [[bag-of-words]]
## Naive Bayes for Document Classification
#### Problem Statement: Why should we use Naive Bayes for Document Classification
#compsci361example Given a [[training data]] set of labeled documents & an unlabeled text document $d$ & set of possible document classes $C$ that $d$ can be labeled with, we want to find the most probable class $c\in C$
$$
c_{MAP} = \underset{c \in C}{\arg\max} \ P(c|d)
$$
- $P(c|d)$ refers to maximising the posterior distribution over the classes $C$ given the example $d$

$$
= \underset{c \in C}{\arg\max} \ \frac{P(d|c)P(c)}{P(d)}
$$

$$
= \underset{c \in C}{\arg\max} \ P(d|c)P(c)
$$
- $P(d|c)P(c)$ refers to maximising the product of the likelihood
#### 1. How should we represent an arbitrary document $d$ in terms of attribute values?
- by taking a sequence of words ([[Document representation]])
#### 2. How should we estimate the probabilities $P(d|c)P(c)$ required by [[Naive Bayes]]?
### Assumptions
1. [[Default assumption]]
2. [[Additional assumption]]
## Summary
- [[Naive Bayes]] allows you to learn a probabilistic function that maps the probability of seeing an example text is from a given class Y