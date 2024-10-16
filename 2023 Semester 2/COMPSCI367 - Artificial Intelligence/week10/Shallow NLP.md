## Writing Systems
- all these languages essentially have the same meaning but just in different representations
- some scripts to not have spacing for words, how do we determine where a word starts or ends
![[Pasted image 20231024165959.png]]

## Preprocessing & Bag of Words
- breaking a [[sentence(s)]] into constituent words
- once you have extracted these base words of [[sentence(s)]], you have key informative words & particles that may also be informative but less important
![[Pasted image 20231024170109.png]]

## [[Information Retrieval (IR)]]
- [[The vector space model]]

## Classification: Probability of a string
![[Pasted image 20231024181746.png]]
- [[language(s)]] is very expensive
$P_{em}(\text{``I don't like the sausage rolls at this tea rooms"})=\,?​$
- we could find documents that have this exact string
	- but this could be a low probability which is not very informative
- Instead, we could break the [[sentence(s)]] into parts, find relevant pages for these terms, then count these documents & calculate proportion of total samples
	- but counting is prone to [[2023 Semester 2/COMPSCI367 - Artificial Intelligence/week10/overfitting]]
![[Pasted image 20231024182526.png]]
$$\frac {Count(x)}{total\ samples}$$
- $x = (x1,...,xn)$
- $x=(don't\ like,sausage\ rolls,tea\ rooms)$

Classifying if this is a positive sentiment or negative sentiment
- $C\tiny 1\normalsize = +ve\ sentiment$
- $C\tiny 2\normalsize = -ve\ sentiment$

$p(C\tiny k \normalsize\ |\ x1,...,xn)$
- bad news because of many possibilities

#### Probability of a +sentiment given our string
$$P(A\ |\ B) = \frac {P(A\cap B)}{P(B)}$$
which is the same as
$$\frac {+sentiment\ \land\ String}{All\ instances/Probability\ of\ getting\ the\ string}$$

