
## Example
#### zh(mandarin) to mi(maori)
find the most probable Maori [[sentence]] given an input sentence in Mandarin
[[The Noisy Channel Model]] interpretation, Maori string has been corrupted & must be recovered
This exemplifies a current research problem in [[Natural Language Processing (NLP)]]
$$\begin{equation}
	\begin{split} 
	\hat {mi}= arg\ max\ p(mi|zh)
		= arg\ max\ \frac {p(zh|mi)\ \cdot p(mi)}{\cancel{p(zh)}}\\
		= arg\ max\ {p(zh|mi)\ \cdot p(mi)}\\
		\end{split}
		\end{equation}$$
- $arg\ max\$ 