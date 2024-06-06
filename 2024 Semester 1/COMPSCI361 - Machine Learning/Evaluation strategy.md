Train/dev/test sets with deep networks![[Pasted image 20240606234602.png]]
- If small dataset (100, 1,000, 10,000 samples)
	- 60%/20%/20%
- If large dataset (> 1,000,000 samples)
	- 98%/1%/1%

Training set, dev set ([[Validation set(s)]]) & test set usually need to come from same distribution (but it is ok varies a bit when gathering a lot of [[training data]])

Make sure dev and test sets come from the same distribution
- If cat & dog must be from cat & dog (not airplanes)
### How does your model do?
[[Bias-Variance vs Fundamental Trade-Off]]/ underfitting vs [[overfit(ting)]]
![[Pasted image 20240606234947.png]]![[Pasted image 20240606234956.png]]
### How to improve learning? [[overfit(ting)]]
Very common problem with [[Deep Learning (DL)]]: [[overfit(ting)]]![[Pasted image 20240606235127.png]]
- [[Regularisation]]
	- Reduces the [[variance]], but increases the [[bias]]
### How does [[Regularisation]] help avoid [[overfit(ting)]]?
1. First intuition:
	- Making some neurons useless to make these predictions $\rightarrow$ simplification
	- [[L1 & L2 regularisation]]
2. Second intuition:
	- Limiting the weight values wil
	