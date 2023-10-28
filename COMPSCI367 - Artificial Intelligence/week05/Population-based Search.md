- [[multi-agent]] [[environment]]
- conducts search by maintaining a [[population]]
- same as [[Local beam Search]] memory
	- they are both fixed size

### Advantages
- Search diversification - introduce randomness & can potentially lead to diverse outputs
	- which may lead to a higher chance of finding a better [[solution(s)]]
	- it does not inherently guarantee diversity due to its susceptibility to issues like local focus, unbalanced exploration, insufficient
- Combination of promising traits in different [[candidate solution]]
	- [[multi-agent]] may share the same information
		> 1 [[agent(s)]] finds shit [[path(s)]]; Another one find a good [[path(s)]]
		> 		Shit [[path(s)]] = We redeploy the agent to a good [[path(s)]] - this could give a possibility of combining promising traits in different [[candidate solution]] - by joining the information that we find: we can easily find a better [[solution(s)]]

## Strategies
1. [[Local beam Search]]
2. [[Genetic Algorithm (GA)]]

## Main Idea
- balance the level of diversity with the immediate benefit/utility of the [[solution(s)]] of the [[population]] that you got
- these searches are NOT [[independent (independence)]]
![[Pasted image 20231023180205.png]]