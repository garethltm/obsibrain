- overlapping area
	![[Pasted image 20231025012028.png]]
- Recall: [[Deriving Bayes Rule]] - 
	- similarly, using the [[Chain Rule]] for [[Joint Entropy]] 
>			$H(X,Y) = H(X) + H(Y|X)$ 
>			we can see that:
>			$H(X,Y) = H(X) + H(Y|X) = H(Y) + H(X|Y)$

Therefore, we can claim:
- $H(X) - H(X|Y) = H(Y) - H(Y|X) = I(X;Y) = I(Y;X)$
	- $I(X;Y) = I(Y;X)$ $\rightarrow$ which represents the middle area
$$I(X;Y) = \displaystyle\sum_{x,y}p(x,y)\ log\frac{p(x,y)}{p(x)\ p(y)}$$

- this basically shows how informative is one variable compared to the other
- Symmetric, non-negative measure of common information in 2 variables
>		how much variables tell you about each other?

- 0 when the variables are independent (no overlaps)
>		independent dice throws

- [[Mutual Information]] grows with the dependence between variables & their [[Entropy (or self-information)]]
>		how dependent are they on each other & how much information do they contain?