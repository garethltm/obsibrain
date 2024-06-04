- sample from the data & train on a subset

#compsci361example Start with a standard deck of 52 cards
1. Sample a random card, put it back & re-shuffle
2. Sample a random card, put it back & re-shuffle
3. Sample a random card, put it back & re-shuffle
4. ...
52. Sample a random card, put it back & re-shuffle
You make a new deck of cards from that 52 samples (bootstrap sample)
- Some cards will be missing, & some cards will be duplicated (because we are putting it back into the deck)
	- So calculations on bootstrap sample will give different results than original data
- However, the bootstrap sample roughly maintains trends:
	- Roughly 25% of the cards will be diamonds
	- Roughly 3/13 of the cards will be face cards
	- There will be roughly 4 10 cards
#### Common use
- compute a statistic based on several bootstrap samples (not necessarily all 52 cards but just a part of it)
	- gives you an idea of how the statistic varies as you vary the data (you get different samples of the same dataset)

### Bootstrap sample of a list of n examples
- A new set of size n chosen independently with replacement![[Pasted image 20240412160921.png]]
- Gives new dataset of n examples, with some duplicated & some missing
	- for large n, approximately 63% of original examples are included (see next slide)
- [[Bagging]]

## 0.632 Bootstrapping
- called this because it is a probability of an instance in a sample

Probability of an arbitrary $\huge x\tiny {i}$ being selected in a bootstrap sample
![[Pasted image 20240412161759.png]]
