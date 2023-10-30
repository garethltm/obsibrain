chooses first better [[state(s)]] from randomly generated neighbours
## Main Idea
- Implementation of [[Stochastic Hill-Climbing]]
- Generating [[successor(s)]] randomly until it finds one which is uphill - finding a neighbour that goes uphill → improves your [[heuristic(s)]] value
	- Very good when a state has many [[successor(s)]]
	- Don't waste time generating them all
		- good because you don't have to generate many neighbours → less generation per iteration