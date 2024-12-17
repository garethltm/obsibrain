is a type of [[Supervised Learning]] algorithm where the output is a discrete value representing one of three or more classes. Unlike [[binary classification]], which involves only two classes, [[multi-class classification]] involves predicting one class from multiple possibilities.

#compsci361example 
a [[multi-class classification]] model could be trained to predict the type of fruit in an image (e.g., apple, banana, cherry, etc.), or to recognize the digit in an image of a handwritten number (0 through 9).

The model is trained using a set of input-output pairs, also known as training examples. Each training example consists of an input vector (or features) and a desired output value (or label). The model learns a function that maps the input to the output for these training examples. Once the model is trained, it can be used to predict the output for new, unseen inputs.
## Common algorithms used for
1. [[Logistic Regression]]
2. [[Decision Tree(s)]]
3. [[Random Forests]]
4. [[gradient boosting]]
5. [[Neural Network (NN)]] and others. 
Some algorithms, like [[Support Vector Machines (SVM)]], are inherently binary classifiers, but can be adapted for [[multi-class classification]] using strategies like [[One-vs-One (OVO)]] or [[One-vs-Rest (OVR)]].