- resembles the [[Annealing]] process used to cool metals slowly to reach an ordered (low-energy) state:

## Main Idea
- allow "bad" moves occasionally, depending on "[[temperature T]]"
- High [[temperature T]]
	- more bad moves allowed, shake the system out of its local minimum
- Gradually reduce temperature according to some [[Typical Annealing Schedule]]

![[Pasted image 20231023172403.png]]
![[Pasted image 20231023172426.png]]

### Probability of accepting a worse [[successor(s)]]
![[Pasted image 20231031003708.png]]

![[Pasted image 20231023173131.png]]
![[Pasted image 20231023173208.png]]
Depending on your problem, your convergence can be very slow. If you have a "big drop" in your temperature scale
	What if you have a lot of local minima on the way?
	You overcome the 1st local minima
		You will start generating a lot of states that won't be accepted - gets lower & lower = you can get stuck in a local minima
## Properties
- convergence might take a VERY long time
- often works very well in practice
	- but usually VERY slow
		- ==slowness comes about because [[temperature T]] must be decreased very gradually to retain optimality==
- [[Simulated Annealing]] & its relatives are a key workhorse in VLSI layout & other [[Optimal]] configuration problems