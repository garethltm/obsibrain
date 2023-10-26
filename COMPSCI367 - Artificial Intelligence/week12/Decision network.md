a [[Probability]] graph model that ==extends a [[Single-stage decision networks (SSDN)]]== to allow both [[Chance nodes]] & [[Decision nodes]] to be parents of [[Decision nodes]]
- graph is acyclic
	- no cycles/loops
- [[Decision nodes]]
- [[no forgetting property]]
- [[Conditional Probability Table (CPT)]] where $P(C\tiny i\normalsize | parents(C\tiny i\normalsize)$) is assigned to every [[Chance nodes]]
- [[Utility function]] u(parents(u)) is given

We will be assuming the [[no forgetting property]] for all [[Decision network]]

>	#Example 
>	Should an [[agent(s)]] take an umbrella?
>	
>	[[Chance nodes]]: 
>	1. Weather: {*norain, rain*}
>	2. Forecast: {*sunny, cloudy, rainy*}
>	[[Decision nodes]]:
>	Umbrella: {0, 1}
>	![[Pasted image 20231026165531.png]]

