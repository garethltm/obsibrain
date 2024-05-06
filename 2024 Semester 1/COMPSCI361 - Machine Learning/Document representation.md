- Document is a sequence of $n$ words (including punctuation)
- $n$ attribute values $<x_{1},\dots ,x_{i},...,x_{n}>$, with the $i$-th attribute representing the $i$-th word position, & its value being the word appearing at the $i$-th position
- #compsci361example "kiwi birds are native species in NZ"
	- $<x_{1}=kiwi,x_{2}=birds,x_{3}=are,x_{4}=native,x_{5}=species,x_{6}=in,x_{7}=NZ,x_{8}=.>$
- Let X be the set of unique attribute values #compsci361example unique words occurring in the [[training data]] set

$$
c_{\text{MAP}} = \underset{c \in C}{\arg\max} \ P(d|c)P(c)
$$

$$
= \underset{c \in C}{\arg\max} \ P(x_1, x_2, ..., x_n|c)P(c)
$$
- $P(x_1, x_2, ..., x_n|c)$ represents the probability that the document is described for this particular word $\rightarrow$ given that the document is related to class $C$