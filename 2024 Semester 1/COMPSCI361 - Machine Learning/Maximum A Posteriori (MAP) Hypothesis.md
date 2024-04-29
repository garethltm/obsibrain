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
- **Equal Probability Assumption**: Sometimes, it’s assumed that every hypothesis is equally probable before observing any data (apriori). In this case, the equation above can be simplified $\rightarrow$ because $P(D|H)$ is often called the likelihood of $D$ given $h$, any hypothesis that maximises $P(D|h)$ is called the [[Maximum Likelihood (ML) Hypothesis]]

- **Simplification**: Under this assumption, the equation for hypothesis testing can be simplified.
- **[[Maximum Likelihood (ML) Hypothesis]]**: This refers to any hypothesis that maximizes the likelihood of the observed data $D$ given the hypothesis $h$, denoted as $P(D|h)$.
- **Constant Probability**: Since every hypothesis is considered equally probable, the prior probability ($P(h)$) can be dropped from the equation, as it is constant for each hypothesis in the set ($H$).

#compsci361example Medical Diagnosis Problem:
- **Hypotheses**:
  - The patient has cancer (**cancer**)
  - The patient does not have cancer (**~cancer**)
### Laboratory Data:
- **Test Outcomes**:
  - Positive (**θ**)
  - Negative (**⊖**)
### Probabilities:
- **P(cancer) = 0.008**
- **P(~cancer) = 0.992**
- **P(θ|cancer) = 0.98**
- **P(θ|~cancer) = 0.03**
### Diagnosis Scenario:
- A patient's lab test returns a positive (**θ**) result.
### Calculations:
- **P(cancer|θ) ≈ P(θ|cancer) * P(cancer)**
  - **= 0.98 * 0.008 = 0.00784**
- **P(~cancer|θ) ≈ P(θ|~cancer) * P(~cancer)**
  - **= 0.03 * 0.992 = 0.02976**
### Conclusion:
- **Does the probability of cancer increase? Yes.**


