![[Pasted image 20240413212242.png]]
- Potential reasons could be:
	- different countries have different jurisdictions/legal systems
- if the missing values doesn't have much influence you could still potentially have a good model (accuracy)
	- which is a problem because you wouldn't be able to detect those issues
there is some relationship that could reveal why some values are missing
- the fact the data are missing is related not to the missing attribute but to some other data in the data set

## Potential Problem
- Bias due to row-wise deletion
	- since we cannot do regression on missing values, we would remove those
		- still could potentially have good datasets for others (US, NZ)