![[Pasted image 20240424170206.png]]
- [[Clustering]] positive & negative instances independently, then apply [[Randomly over-sampling the minority class]] & [[Randomly under-sampling the majority class]] techniques to each single cluster
## Advantage
- Much better representative sample because you are constrained by each class & looking at those structures of that class in the input space
## Does it solve [[overfit(ting)]]?
- No, because if you are choosing an outlier cluster & it chooses that as the representative. It might still overfit to certain noise