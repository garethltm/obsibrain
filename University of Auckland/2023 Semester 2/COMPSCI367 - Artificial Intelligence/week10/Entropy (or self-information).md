- measure of [[uncertainty]] $\rightarrow$ amount of information provided by some data
- $p(x)$ is a [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]] mass function over a random variable $X$ over an alphabet (a set of discrete symbols) $X$:
$$p(x)=P(X=x),x\in X$$
>	tossing 2 dice & taking the sum(what we are interested in), we have the random variable $x = d\tiny 1\normalsize \ +\ d\tiny 2$ and
>		$p(0) = 0$,
>		$p(1) = 0$,
>		$p(2) = \frac {1}{36}$,
>		$p(3) = \frac {2}{36}, ...,p(12) = \frac {1}{36},p(13) = 0, etc.$
>	If we set $X = {2,3,4,5,6,7,8,9,10,11,12}$, being the outcomes that can actually happen, we can eliminate the 0 probabilities

- [[Entropy (or self-information)]] is the average [[uncertainty]] (information, in bits) of a random variable:
$$H(p) = H(X) = -\displaystyle\sum_{x\in X}p(x)\times log \ p(x)$$
![[Pasted image 20231025010549.png]]
- [[Entropy (or self-information)]] of [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]] of mass function = [[Entropy (or self-information)]] of distribution of [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]]
- $-\displaystyle\sum_{x\in X}p(x)$
	- weighted sum
- $-\displaystyle\sum_{x\in X}p(x)\times log \ p(x)$
	- negation of the sum of the [[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]] of X (rolling some result) 
	- multiplied by log ([[University of Auckland/2023 Semester 2/COMPSCI367 - Artificial Intelligence/week09/Probability]] of x)

![[Pasted image 20231025011003.png]]