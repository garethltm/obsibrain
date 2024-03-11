1. Even though what we care about is test error:
	- The test data cannot influence the training phase in any way
2. We're measuring test error to see how well we do on new data:
	- Is used during training, does not measure this
	- You can start to [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] if you use it during training
	- #compsci361example - you are cheating on the exam
3. You also shouldn't change the test set to get the result you want
4. Note the golden rule applies to hypothesis testing in scientific studies
	- Data that you collect can't influence the hypotheses that you test
5. If you want to modify your hypotheses, you need to test on new data
6. Or at least be aware & honest about this issue when reporting results

**COMMON/MAJOR PROBLEM:** 
- Collect more data until you coincidentally get significance level you want
- Try different ways to measure performance, choose the one that looks best
- Choose a different type of model/hypothesis after looking at the test data
