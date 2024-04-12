- a classic [[Boosting]] algorithm for binary [[classification]]

[[AdaBoost]] assumes we have a base binary [[classifier(s)]] that:
- is simple enough that it does not overfit much (moving from underfit towards overfit)
- Can obtain > 50% weighted accuracy on any dataset (need at least 50% accuracy otherwise it's not really improving)

#compsci361example [[Decision Stumps]] or low-depth [[Decision Tree(s)]]
- Easy to modify stumps/trees to use weighted accuracy as score (because it is unlikely to overfit)

## Overview of [[AdaBoost]]
1. Fit a [[classifier(s)]] on the [[training data]] (more likely to underfit - [[Decision Stumps]] which will make m)