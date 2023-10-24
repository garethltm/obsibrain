## Writing Systems
- all these languages essentially have the same meaning but just in different representations
- some scripts to not have spacing for words, how do we determine where a word starts or ends
![[Pasted image 20231024165959.png]]

## Preprocessing & Bag of Words
- breaking a [[sentence]] into constituent words
- once you have extracted these base words of [[sentence]], you have key informative words & particles that may also be informative but less important
![[Pasted image 20231024170109.png]]

## [[Information Retrieval (IR)]]
- [[The vector space model]]

## Classification: Probability of a string
![[Pasted image 20231024181746.png]]
$P_{em}(\text{``I don't like the sausage rolls at this tea rooms"})=\,?​$
- we could find documents that have this exact string
	- but this could be a low probability which is not very informative
- Instead, we could break the [[sentence]] into parts, find releve