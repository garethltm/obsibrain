A [[Kernel function]] $K$ takes vectors in the original space as inputs, & returns the inner product of the vectors in the transformed space (the dot product of data in the transformed space):
$$
K(\vec x_i,\vec x_j) = \Phi(\vec x_i) \cdot \Phi(\vec x_j)
$$
A [[Kernel function]] calculates the similarity between pairs of data points.

Applying the [[Kernel function]] is equivalent to calculating the inner product in the transformed space, but $\Phi$ is never directly calculated (no need to know $\Phi$ explicitly)
- transformation is never directly calculated

A valid [[Kernel function]] is a function that can be used to compute the inner product between 2 feature vectors in a high-dimensional space without explicitly mapping them.
## Possible [[Kernel function]]
You pick the kernel by yourself
- [[Kernel Trick]] to implicitly help you map the low dimensional data into higher dimensional data