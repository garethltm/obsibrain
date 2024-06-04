- allows worsening search steps with a probability that depends on the respective deterioration in evaluation function value

***"The worse a step is, the less likely it would be performed"***![[Pasted image 20231022182721.png]]
- we assign probabilities based on the value we can get from that neighbour
	- if we can improve our [[State(s)]], we give it a high probability. Otherwise, low probability

## Main Idea
- choose the [[successor(s)]] that has the biggest drop in loss may lead to [[Local Optima]] that are not global optima
- To get out of [[Local Optima]], it is necessary to choose other [[successor(s)]]
- We are still favouring [[successor(s)]] that bring faster decrease on the loss - still a [[greedy choice]] approach

Related to: [[Hill-Climbing]]