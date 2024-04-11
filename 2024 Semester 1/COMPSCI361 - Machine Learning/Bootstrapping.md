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
	- Rough