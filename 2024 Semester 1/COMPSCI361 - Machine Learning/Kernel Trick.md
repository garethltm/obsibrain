![[Kernelized Optimization Problem]]
## Motivation
In practice, applying transformation $\Phi$ to the original data is often impractical (high number of features & $\Phi$ can involve polynomial combinations)
- we cannot find a proper transformation that can map the original data to a higher dimension representative (how large the dimensional )
## What [[Kernel Trick]] does
Instead of transforming the input data, and then applying the inner product between pairs of transformed data points, a Kernel function is applied:
![[Pasted image 20240606125337.png]]