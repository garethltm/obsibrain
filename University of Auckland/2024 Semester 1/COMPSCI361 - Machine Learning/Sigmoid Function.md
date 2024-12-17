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
- $y\in \{0,1\}$: binary indicator (0 or 1) if label $c$ is the correct [[classification]] for observation $o$
- $p \in [0,1]$: predicted probability observation $o$ is of class $c$ 
## Optimisation
For a misclassified or barely correct [[training data]] point ($x^{(i)},y^{(i)}$)
$$w\leftarrow w + \lambda (y^{(i)} -\hat {y}^{(i)} )x^{(i)}$$
- $\lambda$ represents the [[Learning rate]]
- $w$ represents the [[Optimal]] value for [[Logistic Regression]]