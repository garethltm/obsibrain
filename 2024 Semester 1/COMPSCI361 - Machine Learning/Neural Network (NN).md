is the ultimate approximator, it can approximate & recover conventional [[Machine Learning (ML)]] methods such as [[Logistic Regression]], [[Support Vector Machines (SVM)]], [[k-nearest neighbor (kNN)]] & [[Decision Tree(s)]]
## Capability of [[Neural Network (NN)]]
If you don't have the hidden layers $\rightarrow$ you cannot approximate the nonlinear functions
#### $M_1$
- 0 hidden layer + linear [[Activation Function]] $\rightarrow$ linear surface
#### $M_2$
- 0 hidden layer + non-linear [[Activation Function]] $\rightarrow$ linear surface ([[Logistic Regression]])
#### $M_3$
- 1 hidden layer + linear [[Activation Function]] $\rightarrow$ combination of linear surface
#### $M_4$
- 1 hidden layer + non-linear [[Activation Function]] $\rightarrow$ non-linear surface (MLP)
## Advantages
- High tolerance to data with a lot of [[Noise]]
- Widely and empirically successful on real-world data
	- #compsci361example hand-written letters
- Algorithm are inherently parallel
- Techniques have recently been developed for the extraction of rules from trained [[Neural Network (NN)]]
- Deep [[Neural Network (NN)]] are powerful
## Disadvantages
- Long training time
- Require to empirically determine
	- #compsci361example the network topology or "structure"
- Difficult to interpret the symbolic meaning behind the learnable weights and hidden units in the network