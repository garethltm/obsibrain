- average a set of deep [[Decision Tree(s)]]
	1. Tend to be one of the best out of the box [[classifier(s)]] - no need to worry about [[hyperparameter(s)]]
	2. Often close to the best performance of any method on the 1st run
	3. Predictions are very fast
### Does [[Averaging]] work if you use trees with the same [[parameters]]?
- Yes, averaging can work even if you use trees with the same parameters.

1. For a **continuous target variable**, each of the trees in an [[Ensemble(s)]] will generate a prediction. [The most naive way to combine the results from trees in an ensemble is to take the mean of all predictions](https://datascience.stackexchange.com/questions/52907/how-are-decision-trees-averaged-in-random-forest)[1](https://datascience.stackexchange.com/questions/52907/how-are-decision-trees-averaged-in-random-forest). This is essentially [[averaging]] the output of each tree.
2. For a **categorical target variable**, each tree acts like a member of a “committee” and casts a vote. [The combined prediction is the category that receives the most votes](https://datascience.stackexchange.com/questions/52907/how-are-decision-trees-averaged-in-random-forest)[1](https://datascience.stackexchange.com/questions/52907/how-are-decision-trees-averaged-in-random-forest). This can be thought of as a form of “[[averaging]]” where the mode (most common value) is taken instead of the mean.

	However, it’s important to note that while the trees might start with the same parameters, the learning process can lead to different structures and splits in the trees, especially when using methods like [[bagging]] or [[boosting]]. This diversity among the trees is what makes the averaging process effective. If all the trees were identical, then [[averaging]] their predictions would just give you the prediction of a single tree. So, while the parameters might start the same, the trees themselves end up being different.

	Remember, thoughtful feature engineering and [[hyperparameter(s)]] tuning are also crucial for improving the performance of [[Decision Tree(s)]]
### Do deep [[Decision Tree(s)]] make independent errors?
- No, with the same [[training data]] you'll get the same [[Decision Tree(s)]]
### 2 key ingredients in [[Random Forests]]
1. [[Bootstrapping]]
2. [[Random trees]]