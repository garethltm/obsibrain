$P(A\ |\ B)$ is the conditional [[probability]] that A will occur, given that B has occurred

The [[belief measure]] in hypothesis $h$ based on [[proposition]] $e$ is called the [[conditional probability]] of $h$ given $e$, written $P(h\ |\ e)$
- [[probability]] of $h$ given $e$

The [[proposition]] e represents certain given experience

The [[conditional probability]] $P(h\ |\ e)=\frac {P(h \land e)}{P(e)}=\frac {hypothesis\ and\ evidence\ TRUE}{prior\ probability\ of\ evidence}$ is the [[agent]]'s [[posterior evidence (posterior probability)]] of $h$.
- $prior\ probability\ of\ evidence$ $\rightarrow$ should be larger
>	[[prior evidence (prior probability)]]: $P(Sunny) = 0.54$
>	
>	[[evidence]] $e$ (new [[evidence]]): $\neg Hot$
>	
>	Other [[evidence]]: 
>	$\begin {equation} \begin {split} P(Sunny \land \neg Hot)=0.19\\ P(\neg Hot)=0.53 \end{split} \end{equation}$
>	[[posterior evidence (posterior probability)]]: $P(Sunny\ |\ \neg Hot) = \frac {0.19}{0.53} \approx 0.36$
>		Belief that it is going to be Sunny is going to drop

## Properties
The following holds for all [[proposition]] $a$ & $b$ & $e$:
- $P(e\ |\ e)=1$
- If $a \land b$ is a contradiction
	- $P(a\ |\ e) + P(b\ |\ e) = P(a\lor b\ |\ e)$
- $P(\neg a\ |\ e)=1-P(a\ |\ e)$
	- they are going to add up to 1
- If a & b are [[logically equivalent (logical equivalence)]] $\rightarrow$ $P(a\ |\ e)=P(b\ |\ e)$
- $P(a\ |\ e)=P(a\ \land \ b\ |\ e) +P(a\ \land \neg b\ |\ e)$
	- $P(Sunny\ |\ NotHot)=P(Sunny\land Windy\ |\ NotHot) +P(Sunny\land NotWindy\ |\ NotHot)$
- $P(a \lor b\ |\ e)=P(a\ |\ e) + P(b\ |\ e)-P(a\land b\ |\ e)$
	- $-P(a\land b\ |\ e)$: to prevent overcounting the intersection
- [[Chain Rule]]
-
Law of