- a [[Planning task]] with the following assumptions:
	-  a finite [[State Space]] → in regards to the series of [[action(s)]] performed to achieve the [[goal(s) - goal state(s)]]
- [[fully observable]] → no need to worry about uncertainty
- [[deterministic]] action → knowing the before & after [[state(s)]] that the [[action(s)]] is performed

>>**basically its saying that everything is in a controlled environment**
- You need a specification of:
    - [[initial state (start state)]]
        - you need a series of [[action(s)]] that the [[agent]] can perform in the [[world]] in order to achieve the [[goal(s) - goal state(s)]]
    - [[goal(s) - goal state(s)]] → marker of success

## 2 [[model(s)]] of planning
1. **Search** → using [[Search Techniques (Search Strategy) (Search Algorithm)]] such as [A*](https://www.notion.so/week04-Local-Search-Stochastic-Search-74d77c6537cc4e0495da5556ded9709f?pvs=21) which requires domain-specific [[heuristic(s)]]
2. **Inference** → uses domain-independent heuristics for inference, but relies on [[Propositional Logic]] which may be space inefficient
![[Pasted image 20231024150510.png]]

### Representing [[Classical Planning]] tasks
> Planning problems are co-related with search
> 	where they are solved in a search
> [[search]]
> [[Logic]]

>[[Classical Planning]] vs [[search]]
>	different [[state(s)]] representation

- [[Classical Planning]]
	- [[state(s)]]: structural information used by [[Classical Planning]] [[algorithm]]
- [[search]]
	- [[state(s)]]: single entity used by the [[search]] [[algorithm]]
![[Untitled 5.png]]