## Summary
- [[Constraint Satisfaction Problem (CSPs)]] are a special kind of problem:
    - [[State(s)]] defined by values of a fixed set of variables
    - [[Goal test]] defined by [[constraint(s)]] on variable values
- [[Backtracking Search]] = [[Depth-First Search (DFS)]] with 1 variable assigned per node
- Variable ordering & value selection [[heuristic(s)]] help significantly

- [[Constraint Satisfaction Problem (CSPs)]] are defined by a set of variables $Xi$, each with a domain $Di$ of possible values, and a set of [[constraint(s)]] C that specify **allowable combinations of values**
- can be formulated as [[Local Search]]
### Additional Information
The aim is to find an assignment of the variables $Xi$ from the domains $Di$ in such a way that none of the [[constraint(s)]] C are violated
> #Example 
> all of the [[constraint(s)]] C are satisfied

### Map Colouring
![[Pasted image 20231023160732.png]]
- Variables:
     `WA, NT, Q, NSW, V, SA, T`
- Domains:
    - $Di = {red, green, blue}$
- [[constraint(s)]]:
    - adjacent regions must have different colours
>	#Example 
>	WA ≠ NT etc,

### n-Queens Puzzle
![[Pasted image 20231023160933.png]]
- Put n queens on an n-by-n chess board so that no 2 queens are attacking each other
- Variables:
	- $Q1, Q2, ..., Qn$
- Domains: 
	- ${1,2,...,n}$
- [[constraint(s)]]:
	- $Qi ≠ Qj$ (cannot be in same row)
	- $|Qi - Qj| ≠ |i-j|$ (or same diagonal)