Suppose $S = {X\tiny 1\normalsize ,..., X\tiny m\normalsize}$ is a set of [[Atomic Propositions (atoms)]], we use $\ohm \tiny s$ to denote the set of [[sample]] on S:
$$\ohm \tiny s\normalsize= {(e\tiny 1\normalsize ,...,e\tiny m\normalsize)\ |\ each\ e\tiny i=X\tiny i\normalsize \ or\ e\tiny i\normalsize =\neg X\tiny i\normalsize \ for\ 1\leq i\leq m}$$
- a [[Probability Distribution]] of a set of [[Atomic Propositions (atoms)]] S, denoted as $P\tiny s$, is a function from $\ohm \tiny s$ into [0,1] such that $$\displaystyle\sum_{w \in \ohm \tiny s}P\tiny s (w) = 1$$
	- we express it as $P(X\tiny 1\normalsize ,..., X\tiny m\normalsize)$
	- $P\tiny s$ $\rightarrow$ a function from the set of [[sample]] into the range [0 to 1] such that:
		- the sum of all [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]] for each of the [[sample]] = 1

- a [[Probability Distribution]] of a set of [[Atomic Propositions (atoms)]] S conditioned on [[Atomic Propositions (atoms)]] $\gamma \tiny 1\normalsize ,...,\gamma \tiny e$ denoted as $P\tiny s |\gamma \tiny 1 ,...,\gamma \tiny e$ is a function from $\ohm \gamma \tiny 1\normalsize ,...,\gamma \tiny e \cup S$ tp [0,1] such that for any $w \in \ohm \gamma \tiny 1\normalsize ,...,\gamma \tiny m$: $$\displaystyle\sum_{r \in \ohm \tiny s}P\tiny {s\ |\ \gamma \tiny 1\normalsize ,...,\gamma \tiny e}\normalsize (w,r) = 1$$
	- we express it as $P(X\tiny 1\normalsize ,..., X\tiny m\normalsize\ |\ \gamma \tiny 1\normalsize ,...,\gamma \tiny e)$
		- $X\tiny 1\normalsize ,..., X\tiny m\normalsize$ $\rightarrow$ represents the hypothesis - combination of different [[Atomic Propositions (atoms)]]
		- $\gamma \tiny 1\normalsize ,...,\gamma \tiny e$ $\rightarrow$ given some [[Atomic Propositions (atoms)]]
	- $(w,r)$ $\rightarrow$ given certain facts
	- $\gamma \tiny 1\normalsize ,...,\gamma \tiny e$ $\rightarrow$ sum of the remaining [[sample]] [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]] are going to add to 1