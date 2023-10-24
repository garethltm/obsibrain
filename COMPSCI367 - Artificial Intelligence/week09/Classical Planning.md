- finding a sequence of [[action(s)]] to get from an [[initial state (start state)]] to a [[goal(s) - goal state(s)]] as a [[Planning task]] with the following assumptions:
	-  a finite [[State Space]] → in regards to the series of [[action(s)]] performed to achieve the [[goal(s) - goal state(s)]] from an [[initial state (start state)]]
	- [[fully observable]] → no need to worry about uncertainty, the [[agent]] can tell which [[state(s)]] we are in
	- [[deterministic]] actions → knowing the before & after [[state(s)]] that the [[action(s)]] is performed, each [[action(s)]] has one outcome, which can be forseen by the [[agent]]
	- nothing changes unless the [[agent]] changes
	- [[goal(s) - goal state(s)]] must be achieved
>>**basically its saying that everything is in a controlled environment**
- You need a specification of:
    - [[initial state (start state)]]
        - you need a series of [[action(s)]] that the [[agent]] can perform in the [[world]] in order to achieve the [[goal(s) - goal state(s)]]
    - [[goal(s) - goal state(s)]] → marker of success
- [[Task description]]
![[Pasted image 20231024150510.png]]
## 2 [[model(s)]] of planning
1. **Search** → using [[Search Techniques (Search Strategy) (Search Algorithm)]] such as [A*](https://www.notion.so/week04-Local-Search-Stochastic-Search-74d77c6537cc4e0495da5556ded9709f?pvs=21) which requires domain-specific [[heuristic(s)]]
2. **Inference** → [[SATPlan]] uses domain-independent [[heuristic(s)]] for [[inference(s)]], but relies on [[Propositional Logic]] which may be space inefficient
 
