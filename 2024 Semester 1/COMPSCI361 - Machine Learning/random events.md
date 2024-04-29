Sample space $\Omega$: The set of all the outcomes of a random experiment. 
Here, each outcome $\omega \in \Omega$ can be thought of as a complete description of the state of the real world at the end of the experiment.

Set of events (or event space) $F$: A set whose elements $A \in F$ (called events) are subsets of $\Omega$ (i.e., $A \subseteq \Omega$) is a collection of possible outcomes of an experiment.

Probability measure: A function $P : F \rightarrow \mathbb{R}$ that satisfies the following properties:
- $P(A) \ge 0$, \for all $A \in F$
- $P(\Omega) = 1$
- If $A_1, A_2, \ldots$ are disjoint events 
	#compsci361example $A_i \cap A_j = \emptyset$ whenever $i \neq j$), then $P\left(\bigcup_{i} A_{i}\right) = \sum P(A_{i})$

*Note: Probability can have a range between 0 and 1.*
