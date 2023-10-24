- overlapping area
	![[Pasted image 20231025012028.png]]
- Recall: [[Deriving Bayes Rule]] - 
	- similarly, using the [[Chain Rule]] for [[Joint Entropy]] 
>			$H(X,Y) = H(X) + H(Y|X)$ 
>			we can see that:
>			$H(X,Y) = H(X) + H(Y|X) = H(Y) + H(X|Y)$

Therefore, we can claim:
- $H(X) - H(X|Y) = H(Y) - H(Y|X) = I(X;Y) = I(Y;X)$
	- $I(X;Y) = I(Y;X)$ $\rightarrow$ represents the middle are