- [[Cluster(s)]]
	- Similar (or related) to one another within the same group (same labels)
	- Dissimilar (or unrelated) to objects in other groups
- [[Clustering]] ([[Cluster(s)]] analysis, data segmentation,...)
	- Finding similarities between data according to the characteristics found in the data & grouping similar data objects into [[Cluster(s)]]
- the best [[Clustering]] is hard to define (because there is no ground truth)
	- We don't have a [[test error]]
	- Generally, there is no best method in [[Supervised Learning]] (you want to discover something)
		- so there are lots of methods, we will focus on important/representative ones
## Motivation
#compsci361example Classifying Cancer Types
- We collected gene expression data for 8 cancer patients, can you find the types of cancer in the data?![[Pasted image 20240515163716.png]]
## General idea
![[Pasted image 20240515164136.png]]
![[Pasted image 20240515164111.png]]
- Input: set of [[instance(s)]] described by $d$ features
- Output: an assignment of [[instance(s)]] to 'groups' (no target class)
- Unlike [[classification]], we are not given the 'groups'
	- #### Task: Algorithm must discover groups
- #compsci361example groups we might discover in e-mail spam:
	- 'Lucky winner' group
	- 'Weight loss' group
	- 'I need your help' group
	- 'Mail-order bride' group

#compsci361questions 
## What [[Clustering]] does
- 2 data points that are similar are enclosed in a space - everything close is 1 cluster
- Detect and remove outliers![[Pasted image 20240413224824.png]]
## Potential Problem
1. Information loss
2. There might be some outliers beyond the domain
## Typical Applications
- You could want to know what the groups are
- You could want to find the group for a new example $x_i$
- You could want to find examples related to a new example $x_i$
	- give examples that are closely related
- You could want a prototype example for each group
	- give the most representative example for that group
## Applications - Data Understanding
- Biology
	- taxonomy of living things: kingdom, phylum, class, order, family, genus & species
- Information retrieval
	- document clustering
- Land use
	- Identification of areas of similar land use in an earth observation database
- Marketing
	- Help marketers discover distinct groups in their customer bases, & then use this knowledge to develop targeted marketing programs
- City-planning
	- Identifying groups of houses according to their house type, value, & geographical location
- Earth-quake studies
	- Observed earth quake epicenters should be clustered along continent faults
- Climate
	- understanding earth climate, find patterns of atmospheric & ocean changes
## Applications - [[Preprocessing & Evaluation]]
1. Summarizing
	- [[Preprocessing & Evaluation]] for [[Regression]], [[Principal Components Analysis (PCA)]], [[classification]] & association analysis
2. Compression
	- Image processing: colour quantization (computer graphics) ( #compsci361example task of reducing the colour palette of an image to a fixed number of colours) - merging colour palettes
3. Outlier detection
	- Outliers are often viewed as those "far away" from any [[Cluster(s)]]