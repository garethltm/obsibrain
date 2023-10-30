- an alternative method to [[Local beam Search]] by introducing randomness ([[Stochastic]])
- [[Stochastic Beam Search (SBS)]] does not have memory as it is a fixed size
	- choose M [[successor(s)]] using [[Boltzmann distribution]]
	![[Pasted image 20231023180406.png]]

A Darwinian interpretation:
- `val(x)` represents the [[fitness]] of a [[candidate solution]]
- the stronger x is, the more likely it "survives"