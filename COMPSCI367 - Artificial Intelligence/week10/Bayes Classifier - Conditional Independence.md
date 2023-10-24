$$C\tiny MAP\normalsize = arg\ max\ P(x,\large c\tiny k\normalsize)$$
- where $\large c\tiny k\normalsize$ ∈ C
- But, need to know for each sentiment, the [[probability]] it will produce any bag (combination) of terms
- The bad thing about [[Natural Language Processing (NLP)]] is that it's productive. The good thing about this is that it leads to expressivity
- Let's pretend that the words in the bag are independent given the class
>	given that it's a bad (or good) review, the [[probability]] of producing "sausage roll" is independent of the [[probability]] of producing "tea rooms".
>		where in the real world, they won't be independent
>	We are assuming independence for the purpose of creating this classifier
>	![[Pasted image 20231025001647.png]]

