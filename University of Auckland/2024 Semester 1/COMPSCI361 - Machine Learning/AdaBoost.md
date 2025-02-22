- a classic [[Boosting]] algorithm for [[binary classification]]

[[AdaBoost]] assumes we have a base binary [[classifier(s)]] that:
- is simple enough that it does not [[overfit(ting)]] much (moving from underfit towards [[overfit(ting)]])
- Can obtain > 50% weighted [[Accuracy]] on any dataset (need at least 50% [[Accuracy]] otherwise it's not really improving)

#compsci361example [[Decision Stumps]] or low-depth [[Decision Tree(s)]]
- Easy to modify stumps/trees to use weighted [[Accuracy]] as score (because it is unlikely to [[overfit(ting)]])

## Overview of [[AdaBoost]]
1. Fit a [[classifier(s)]] on the [[training data]] (more likely to underfit - [[Decision Stumps]] which will make mistakes)
2. Give a higher weight to examples that the [[classifier(s)]] got wrong - higher weight such as duplicating
3. Fit a [[classifier(s)]] on the weighted [[training data]]
4. Go back to Step (2) - Weight gets exponentially larger each time you are wrong
Final prediction: weighted vote of individual [[classifier(s)]] predictions
- Trees with higher (weighted) accuracy get higher weight

## Main idea
giving these examples that are wrong with higher weightage to allow the [[classifier(s)]] to pay more attention to
- in a way it is still sort of [[overfit(ting)]] in some way - getting better on the [[training data]]

#compsci361questions Are [[Decision Stumps]] a good base [[classifier(s)]]?
- They tend not to [[overfit(ting)]] (usually underfit)
- Easy to get > 50% weighted [[Accuracy]] (because it is just a [[Decision Stumps]] - 2 decisions)

## Base [[classifier(s)]] that don't work
- Deep [[Decision Tree(s)]] (no errors to boost) - if you don't get errors, nothing will improve
- [[Decision Stumps]] with infogain (does not guarantee > 50% weighted [[Accuracy]] - because oh having clean splits into positive class & negative class. If you instead took accuracy as a splitting criterion $\rightarrow$ can guarantee good [[Accuracy]])
- Weighted logistic [[Regression]] (does not guarantee > 50% weighted [[Accuracy]])

## [[AdaBoost]] with shallow [[Decision Tree(s)]] gives fast/accurate [[classifier(s)]]
- Classically viewed as one of the best off-the-shelf [[classifier(s)]]
- Procedures originally came from ideas in [[Learning Theory]]

## Many attempts to extend theory beyond binary case
- Led to [[gradient boosting]]