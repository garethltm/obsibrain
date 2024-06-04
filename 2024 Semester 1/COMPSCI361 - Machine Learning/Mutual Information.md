- an information-theoretic measure about the amount of information by which our knowledge about the categories increases when we are told what the [[cluster(s)]] are
- It is 0 if the [[Clustering]] is random with respect to category membership
	$$
I(C, G) = \sum_{i} \sum_{j} p(C_i, G_j) \log\left(\frac{p(C_i, G_j)}{p(C_i) \cdot p(G_j)}\right)
$$

$$
= \sum_{i} \sum_{j} \frac{|C_i \cap G_j|}{n} \log\left(\frac{n \cdot |C_i \cap G_j|}{|C_i| \cdot |G_j|}\right)
$$
