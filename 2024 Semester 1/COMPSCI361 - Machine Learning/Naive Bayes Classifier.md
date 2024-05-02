Applies to learning tasks where each instance x is described by a conjunction of attribute values $<a\tiny{1} \normalsize , a\tiny{2} \normalsize, \dots ,a\tiny{n}>$ & where the target function $f(x)$ can take on any value from some finite set V
- the most probable target value is:

- [[Naive Bayes Classifier]] solves the spam problem
$$
V_{\text{MAP}} = \underset{v_j \in V}{\operatorname{arg\,max}} \ P(v_j | a_1, a_2, ..., a_n)
= \underset{v_j \in V}{\operatorname{arg\,max}} \ P(a_1, a_2, ..., a_n; v_j)
$$
$$= \underset{v_j \in V}{\operatorname{arg\,max}} \ P(a_1, a_2, ..., a_n | v_j)P(v_j) \\
$$