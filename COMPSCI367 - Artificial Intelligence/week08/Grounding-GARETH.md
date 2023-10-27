changing a variable into a constant
- Substitution ($\frac {x}{t}$) → replacing variable x with the term t
- A **[[sentence]]** without any [[quantifier(s)]] is a [[proposition]]

>	#Example 
>	In Greedy(y) we cannot say that it is True/False;![[Pasted image 20231024013638.png]]

1. [[Instantiation]]
2. A strategy that converts a [[First-Order KB]] into a [[Propositional Knowledge Base]]

### Rule 1: Existential [[instantiation]]
- [[Skolem constant]]

### Rule 2: Universal [[instantiation]]
- may be applied many times to infer infinitely many [[sentence]]$$\frac{\forall y:x(y)}{\text{Subst}(\{y/t\},x(y))}$$
Essentially, we can turn $\forall x: King(x)\ into\ King(John)$
- where $x$ can be anything, John, Richard, etc.

> Repeated applications of Existential/Universal Instantiation would produce a new [[Knowledge Base (KB)]] that contains [[sentence]] without [[quantifier(s)]] (a [[proposition]])

For any [[sentence]] φ, $KB ⊧ φ$ then $KB’ ⊧ φ$ - vice versa; it has the same [[semantics]]
- KB’ essentially has no [[quantifier(s)]], therefore it is a [[proposition]]
- KB’ can potentially be an infinite set