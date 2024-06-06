$$
l(y^{(i)}, \hat{y}^{(i)}) = \max(0, 1 - y^{(i)}\hat{y}^{(i)})
$$
$$
L(w) = \frac{1}{n} \sum_{i} \max(0, 1 - y^{(i)} \hat{y}^{(i)})
$$

$$
\frac{\partial L}{\partial w} = - \sum_{i=1}^{n} y^{(i)} x^{(i)} \text{ if } y^{(i)} \hat{y}^{(i)} < 1
$$

