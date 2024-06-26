![[Pasted image 20240424173633.png]]
- find [[principal subspace]] (denoted by the magenta line) such that the orthogonal projection of the data (red) points onto this subspace
## What happens?
- maximizes the [[variance]] of the projected (green) points
- minimizes the sum-of-squares of the projection errors, indicated by the blue lines
	- we want to find the best fitting line
## How it happens?
![[Pasted image 20240424174053.png]]
- We find the [[eigenvectors (principal components)]] & [[eigenvalues]] of the covariance matrix of the input attributes![[IMG_106235EA91B4-1.jpeg]]
## How can it be accomplished
- rotating the axes (if the data is centered)
## Steps
Given $n$ data instances (each a vector in d-dimensions), find $k \le d$ [[eigenvectors (principal components)]] that can be best used to represent the data
1. [[Normalization]] input data: each attribute falls within the same range
2. Compute [[eigenvectors (principal components)]] using [[eigenvalues]] decomposition of the covariance of the normalized data
3. The input data is a linear combination of the [[eigenvectors (principal components)]] - we only want to use $k$
4. The [[eigenvectors (principal components)]] are sorted in order of decreasing "significance" or strength #compsci361example measured by the [[eigenvalues]]
5. Since the [[eigenvectors (principal components)]] are sorted, the size of the data could be reduced by eliminating $d-k$ weak [[eigenvectors (principal components)]] #compsci361example those with low [[variance]] (keeping only the top $k$ features)
The resulting attributes are uncorrelated
## How can you apply [[Principal Components Analysis (PCA)]] on categorical data?
- You have to transform your categorical data into binary features $\rightarrow$ [[Normalization]] $\rightarrow$ apply [[Principal Components Analysis (PCA)]]
## Summary
- reducing a 2D space into 1
- 1st component is most important because it explains the variability in the data