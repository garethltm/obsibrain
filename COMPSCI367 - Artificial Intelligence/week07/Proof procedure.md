If there is a proof of g starting from S then `S ⊦ g`

#### Proof procedure that are both [[Sound (Proposition)]] & [[Complete (Proposition)]]
1. **Forward Chaining**
    1. not very ideal/efficient
2. **SLD Resolution** (Backward chaining) - iteratively replace goals with subgoals; try to get head with an empty body
    1. potentially more efficient