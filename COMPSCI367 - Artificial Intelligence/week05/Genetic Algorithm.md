- [[Search Techniques (Search Strategy) (Search Algorithm)]] inspired by [[genetics]] & [[evolution]] in biology
- a variation of [[Stochastic Beam Search (SBS)]] that generates every [[successor(s)]] using 2 [[candidate solution]]

![[Pasted image 20231023181930.png]]

## Main Idea
- to apply the [[evolution]] paradigm as a [[Search Techniques (Search Strategy) (Search Algorithm)]], we need:
	1. [[candidate solution]] representation: the most common representation of a [[candidate solution]] in S is a (fixed-length) string of characters in a finite alphabet. They are also called chromosomes
	2. [[fitness]]
	3. [[crossover operation]]
	4. [[mutation operation]]

### Summary
- [[Population-based Search]] conducts search by maintaining & updating a collection of [[candidate solution]]
- [[Local beam Search]] is an adaptation of [[Iterative Best Improvement (IBI)]] by maintaining M > 1 [[candidate solution]]
- [[Stochastic Beam Search (SBS)]] aims to avoid [[Local beam Search]] concentration on a narrow [[path(s)]] by using [[Boltzmann distribution]]
