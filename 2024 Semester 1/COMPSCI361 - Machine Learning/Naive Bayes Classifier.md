Applies to learning tasks where each instance x is described by a conjunction of attribute values $<a\tiny{1} \normalsize , a\tiny{2} \normalsize, \dots ,a\tiny{n}>$ & where the target function $f(x)$ can take on any value from some finite set V
- [[Naive Bayes Classifier]] solves the spam problem
- $<a\tiny{1} \normalsize , a\tiny{2} \normalsize, \dots ,a\tiny{n}>$ is the [[posterior evidence (posterior probability)]] given the attribute values you have seen for that particular instance
	- #compsci361example can represent color, height,...

- the most probable target value is:
$$
V_{\text{MAP}} = \underset{v_j \in V}{\operatorname{arg\,max}} \ P(v_j | a_1, a_2, ..., a_n)
$$
$$= \underset{v_j \in V}{\operatorname{arg\,max}} \ \frac{P(a_1, a_2, ..., a_n | v_j)P(v_j)}{P(a_1, a_2, ..., a_n)}\\
$$
$$= \underset{v_j \in V}{\operatorname{arg\,max}} \ P(a_1, a_2, ..., a_n | v_j)P(v_j)$$
- 
- We can remove $P(a_1, a_2, ..., a_n)$ as normalisation is not necessary
