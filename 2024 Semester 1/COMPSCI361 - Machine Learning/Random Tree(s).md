- it does the same as [[Bootstrapping]] but does it on a feature level

For each split in a [[Random Tree(s)]] model
- Randomly sample a small number of possible features (typically $\sqrt {d}$) - where d is the number of features
- Only consider these random features when searching for the optimal rule

Splits tend to use different features in different trees
- They will still overfit, but hopefully 

#compsci361example ![[Pasted image 20240412162111.png]]
![[Pasted image 20240412162123.png]]