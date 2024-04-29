In many learning scenarios, the learner considers some set of candidate hypotheses **H** and is interested in finding the most probable hypothesis **h** in **H** given the observed [[training data]] **D**.

Any maximally probable hypothesis is called [[Maximum A Posteriori (MAP) Hypothesis]] **$h_{MAP}$**.
$$
h_{MAP} = \arg\max_{h \in H} P(h|D)
$$
- find the algorithm that gives the maximum prior [[probability]] after observation


By [[2024 Semester 1/COMPSCI361 - Machine Learning/Bayes Theorem|Bayes Theorem]],
$$
= \arg\max_{h \in H} \frac{P(D|h)P(h)}{P(D)}
$$

*Note that we can drop $P(D)$ because it is a constant independent of $h$*:
$$
= \arg\max_{h \in H} {P(D|h)P(h)}
$$
## Choosing a Hypothesis
Sometimes it is assumed that every hypothesis is equally probable apriori
In this case, the equation above can be simplified $\rightarrow$ because $P(D|H)$ is often called the likelihood of $D$ given $h$, any hypothesis that maximises $P(D|h)$ is called the maximum likelihood (ML) Hypothesis
