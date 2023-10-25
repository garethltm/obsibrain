- a theory that gives us tools for reliably reasoning about [[uncertainty]]
- is a [[calculus of belief]]
>	There is a 80% [[probability]] of raining expresses a belief based on past experience
- [[Probability Theory]] is the study of how [[knowledge]] affects belief
	- new [[evidence]], revise your belief
- The [[probability]] of a hypothesis $\alpha$ is a scale of the [[agent]]'s belief in $\alpha$ in the range [0,1] 
	- 0 is no chance to occur
	- 1 is certain to occur

## Example
Let $X\tiny 1\normalsize ,...,X\tiny d$ be [[Atomic Propositions (atoms)]]
>	Sunny means outlook will be sunny
>	Hot means high temperature

The sample space $\ohm$ over these [[Atomic Propositions (atoms)]] contains all possible [[interpretation]]. 
>[[sample]] over Sunny, Hot
![[Pasted image 20231025132516.png]]

A [[proposition]] describes a [[constraint(s)]] on [[Atomic Propositions (atoms)]]
>	1. $\alpha \tiny 1\normalsize: \neg Hot$
>		$e \tiny 2\normalsize \vDash \alpha \tiny 1,e \tiny 4\normalsize \vDash \alpha \tiny 1$ 
>				$e \tiny 2\normalsize \& \$e \tiny 4\normalsize$ 
>	1. $\alpha \tiny 2\normalsize: \neg Sunny \lor \neg Hot$
>		$e\tiny 2\normalsize \vDash \alpha \tiny 2\normalsize ,e\tiny 3\normalsize \vDash \alpha \tiny 2\normalsize ,e\tiny 4\normalsize \vDash \alpha \tiny 2\normalsize$
>				either one of them is False
