- it does the same as [[Bootstrapping]] but does it on a feature level

For each split in a [[Random Tree(s)]] model
- Randomly sample a small number of possible features (typically $\sqrt {d}$) - where d is the number of features
- Only consider these random features when searching for the optimal rule
- 