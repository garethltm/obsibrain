Sample space $\Omega$: The set of all the outcomes of a random experiment. (ALL POSSIBLE OUTCOMES)
Here, each outcome $\omega \in \Omega$ can be thought of as a complete description of the state of the real world at the end of the experiment.

Set of events (or event space) $F$: A set whose elements $A \in F$ (called events) are subsets of $\Omega$ (i.e., $A \subseteq \Omega$) is a collection of possible outcomes of an experiment.

Probability measure: A function $P : F \rightarrow \mathbb{R}$ that satisfies the following properties: 
($\mathbb{R}$ because *[[Probability]] can have a range between 0 and 1.*
 
- $P(A) \ge 0$, \for all $A \in F$
- $P(\Omega) = 1$ (probability of any outcome happening is certain)
- If $A_1, A_2, \ldots$ are disjoint events 
	#compsci361example $A_i \cap A_j = \emptyset$ whenever $i \neq j$), then $P\left(\bigcup_{i} A_{i}\right) = \displaystyle\sum_{i} P(A_{i})$

#compsci361example Consider the event of tossing a six-sided die. 
The sample space is $S = \{1,2,3,4,5,6\}$. We can define different event spaces on this sample space. For example, the simplest event space is the trivial event space $F = \{\emptyset, \Omega\}$. (either you roll or don't roll)

Another event space is the set of all subsets of $\Omega$. For the first event space, the unique probability measure satisfying the requirements above is given by $P(\emptyset) = 0$, $P(\Omega) = 1$. 
($P(\Omega) = 1$ because the dice will always have a face to show when rolled)

For the second event space, one valid probability measure is to assign the probability of each set in the event space to be $\frac{i}{6}$ where $i$ is the number of elements of that set; for example,
$P(\{1,2,3,4\}) = \frac{4}{6}$ and $P(\{1,2,3\}) = \frac{3}{6}$.


