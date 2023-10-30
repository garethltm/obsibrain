- [[Local Search]] strategy where randomisation plays a prominent role:
	- Initialisation: Random start
	- Tie breaking: Random tie breaking
	- Step function:
		> random ordering of [[successor(s)]] ([[First Choice Hill-Climbing]]), random [[Tabu Search]] tenure
- ==[[Local Search]] strategies== introduced earlier ==can all be extended== by [[Stochastic Local Search (SLS)]]

## Types
- [[First Choice Hill-Climbing]] - choose first better random child
- [[Stochastic Hill-Climbing]] - choose probabilistically from among better children based on their [[fitness]]
- [[Random Walk Hill-Climbing]] - choose probabilistically between best child & random child
- [[Random-Restart Hill Climbing]] - do any [[Hill-Climbing]] method with random restarts to try to get a better result
- [[Simulated Annealing]] - [[First Choice Hill-Climbing]] with a [[Stochastic]] chance of choosing a worse node. The chance of choosing a worse node reduces over time with the [[temperature T]] schedule

