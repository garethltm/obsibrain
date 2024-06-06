- Sigmoid Unit ($\sigma$) is selected as the [[Activation Function]]
$$\hat{y} = \sigma \left( \sum_{j} w_j x_j + b \right)
= \frac{1}{1+exp{(-\left(\sum_{j} w_j x_j + b\right)})}
$$
## [[Activation Function]] 
- Training: [[Sigmoid Function]]
- [[inference(s)]]: [[Sigmoid Function]]
## [[Loss Function]]
[[Loss Function]] compared to cross [[entropy]] function
$$l = -(y \ln(p) + (1 - y) \ln(1 - p))$$
- $y\in \{0,1}\$