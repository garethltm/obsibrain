[[Ensembles]] are [[classifier(s)]] that have [[classifier(s)]] as input
- still outputs a prediction
### Some methods
1. [[Averaging]]
2. [[Boosting]]
3. [[Bootstrapping]]
4. [[Bagging]]
5. [[Cascading]]
6. [[Random Forests]]
7. [[Stacking]]

[[Ensembles]] methods often have higher accuracy than the input [[classifier(s)]]

#### [[Fundamental Trade-Off]] (bias variance, training approximation)
1. $E\tiny {train}$: How small can you make [[training error]]
2. $E\tiny {approx}$: How well [[training error]] approximates the [[test error]]

## Main idea
Combining models to get a better prediction for the base [[classifier(s)]] that we input by making an average of the [[classifier(s)]]

## Goal
The [[Ensembles]] [[classifier(s)]]:
1. does much better on one of these than the individual [[classifier(s)]]
2. doesn't do too much worse on the other
