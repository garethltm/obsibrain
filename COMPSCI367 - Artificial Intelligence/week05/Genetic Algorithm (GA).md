- [[Search Techniques (Search Strategy) (Search Algorithm)]] inspired by [[genetics]] & [[evolution]] in biology
- a variation of [[Stochastic Beam Search (SBS)]] that generates every [[successor(s)]] using 2 [[candidate solution]]
- [[Genetic Algorithm (GA)]] does not converge quickly because of the amount of diversity
- [[Genetic Algorithm (GA)]] does not have memory as it is a fixed-size of [[population]] M

![[Pasted image 20231023181930.png]]

## Fundamentals
- to apply the [[evolution]] paradigm as a [[Search Techniques (Search Strategy) (Search Algorithm)]], we need:
	1. [[candidate solution]] representation: the most common representation of a [[candidate solution]] in S is a (fixed-length) string of characters in a finite alphabet. They are also called chromosomes
	2. [[fitness]]
	3. [[crossover operation]]
	4. [[mutation operation]]

### Summary
- [[Population-based Search]] conducts search by maintaining & updating a collection of [[candidate solution]]
- [[Local beam Search]] is an adaptation of [[Iterative Best Improvement (IBI)]] by maintaining M > 1 [[candidate solution]]
- [[Stochastic Beam Search (SBS)]] aims to avoid [[Local beam Search]] concentration on a narrow [[path(s)]] by using [[Boltzmann distribution]]
#### Framework
- [[Genetic Algorithm (GA)]] maintains a [[population]] of [[candidate solution]]
- Chromosomes are representations of [[candidate solution]] that determines [[fitness]]
- [[crossover operation]] & [[mutation operation]] for generating offspring

What are the weakness of [[Local beam Search]] algorithm?
- sometimes the search would only concentrate on a certain solution's neighbour depending on the fitness values

What modification to the algorithm you can do to mitigate this problem?
- adding some randomness to the search