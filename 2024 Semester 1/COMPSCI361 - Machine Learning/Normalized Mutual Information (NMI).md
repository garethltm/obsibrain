[[2024 Semester 1/COMPSCI361 - Machine Learning/Mutual Information|Mutual Information]] is 1 for perfect [[Clustering]], but also 1 for $k=n$ (same problem as with [[Purity]])

[[Normalized Mutual Information (NMI)]] in range [0,1], and penalizes for too many [[cluster(s)]]:
$$
NMI(C, G) = \frac{I(C, G) \cdot 2}{H(C) + H(G)}
$$
where $H$ is the entropy $H(C) = - \sum_i p(C_i) \log p(C_i) = - \sum_i \frac{|C_i|}{n} \log \frac{|C_i|}{n}$
#compsci361example ![[Pasted image 20240604173102.png]]