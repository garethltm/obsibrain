Data are not always available
- Many tuples have no recorded value for several attributes
- #compsci361example customer income in sales data

Missing data may be due to:
1. Equipment malfunction
2. Inconsistent with other recorded data & thus deleted (Deleted because we thought it was inconsistent $\rightarrow$ creates empty values)
3. Data not entered due to misunderstanding (Data may not be applicable to you $\rightarrow$ leaves empty)
4. Certain data may not be considered important at the time of entry
5. Data history or changes of the data not recorded (Forget to update data)
## [[Incomplete (Missing) Data]] may need to be inferred
- Some algorithms cannot handle those values $\rightarrow$ [[Linear Regression]] requires all values to be present
## What to consider when handling [[Incomplete (Missing) Data]]?
1. [[Missing completely at random (MCAR)]]
2. [[Missing at random (MAR)]]
3. [[Missing not at random (MNAR)]]
## How to handle [[Incomplete (Missing) Data]]
##### Problem![[Pasted image 20240413213542.png]]

##### Solution
1. Fill in the missing data manually![[Pasted image 20240413213624.png]]
2. Fill in automatically (this is more feasible rather than the manual entry for large datasets) 
	1. a global constant (since they are all of the same type) ![[Pasted image 20240413213930.png]]
		- However, it might still work for [[Classification]] problem & it affects the class variable
	2. the attribute mean (more general case, where there are mixed values & continuous variable) ![[Pasted image 20240413214300.png]]
		- Done automatically by many implementations $\rightarrow$ Default assumption
		- Changes relationship with other variables $\implies$ bias in data (because you are calculating the mean based on a variable that may be dependent)
		- The mean is calculated based on observed values in that variable (you calculate the mean based on the available values at the end)
	3. the attribute mean of the samples belonging to the same class (replacing the value that has a similar target variable) - a **BETTER** way to do it![[Pasted image 20240413214545.png]]
		- Might change relationship with other variables other than class $\implies$ bias in data (we need to explore the whole data in such a way where we keep those underlying relations)
		- There might be relationship between X' & other features in combination (you are only looking at a single pairwise relationship)
	4. the most probab