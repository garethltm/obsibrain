- [[Perceptron Learning]] finds [[decision boundary]] if classes are [[Linearly Separable Data]]

 $l(y^{(i)}, \hat{y}^{(i)}) = \max(0, 1 - y^{(i)}\hat{y}^{(i)})$
- Intuition for updating weight based on error over one sample:
	1. If $\hat {y}^{(i)} = y^{(i)},\ l = 0$ 
		- [[Loss Function]] equals 0: the lowest point $w$, no update needed
	2. $\hat {y}^{(i)} \ne y^{(i)}$ and $y^{(i)}=1,\ l > 0$
		- [[Loss Function]] more than 0: weight must be increased so that $\hat {y}^{(i)}$ will increase = $w\leftarrow w + \lambda ( y^{(i)} x^{(i)})$
	3. $\hat {y}^{(i)} \ne y^{(i)}$ and $y^{(i)}=-1,\ l > 0$
		- [[Loss Function]] less than 0: weight must be decreased so that $\hat {y}^{(i)}$ will decrease = $w\leftarrow w - \lambda ( y^{(i)} x^{(i)})$
- **If [[Loss Function]] bigger than 1 than there is some error**
	