- [[Definite Clause Inference Engine]] need to handle queries of form `ask b` where b is an [[Atomic Propositions (atoms)]]

## Implementing a definite clause inference engine
- [[Inference engines (IE)]] produces a PROOF
>Think of an inference engine as a detective. 
>
>The detective has a set of facts (the crime scene, evidence, witness statements) and a goal (to find out who committed the crime). 
>
>The detective uses logical reasoning (the inference rules) to connect the facts and reach a conclusion (the proof). 
>
>If the detective can show that the conclusion logically follows from the facts, then they have solved the case.


## Abstract Idea
Proof procedure → If there is a proof of g starting from S then `S ⊦ g`
- **[[Sound]]** 
- **[[COMPSCI367 - Artificial Intelligence/week02/Complete]]**
`S ⊦ g` (Proof procedures) that are both **Sound** & **Complete**

1. **Forward Chaining**
    1. not very ideal/efficient
2. **SLD Resolution** (Backward chaining) - iteratively replace goals with subgoals; try to get head with an empty body
    1. potentially more efficient