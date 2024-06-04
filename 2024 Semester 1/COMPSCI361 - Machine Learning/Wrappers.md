- the [[Attribute (Feature) selection]] is "wrapped" in a search procedure that:
1. Generates a candidate subset of attributes
2. Trains & evaluates a model with candidate subset on a [[Validation set(s)]]
3. Add and/or remove attributes from the subset until predictive performance of the model improves
## Advantages & Disadvantages
1. High accuracy but computationally expensive
2. Risk of [[overfit(ting)]], especially if the same learning algorithm for subset selection & main learning task (if different algorithm $\rightarrow$ less likely)![[Pasted image 20240426174959.png]]