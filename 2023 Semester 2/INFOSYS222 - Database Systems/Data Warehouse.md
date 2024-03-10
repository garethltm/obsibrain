- Businesses generate massive amount of data from many different sources that we may not keep track of
- basically multiplying all the values to get the number of records
- Idea of what should you do with data that has already been used for a recent transaction
- Focused on query performance

## Motivation
- Business generates massive amount of data from many different sources
- Most of the data remains unused in the long term
- Harness data to drive strategic decisions ([[Business Intelligence]])

### Properties
- Subject Oriented
	- Define business purpose
		>this [[Data Warehouse]] may have [[Star Schema]] for its purpose
- Integrated → you get data from different sources so you want them to be cohesive in a way/synchronized
	- Disparate sources, we want a consistent outcome
- Non-volatile → Don't want to delete
	- Permanent record of the past
- Time-variant → Studying how things are changing over time
	- Focus on change over time
Time is a default [[Dimension]]

### Implications
- Subject Oriented → Get useful columns from tables
	- Exclude data not relevant to the subject
- Integrated
	- Consistent naming; Common measures; Identical Coding (1 Identifier)
- Non-volatile
	- Add but don't 
Properties causes Implications

## Architecture
1. [[Basic]]
2. [[Basic with Staging]]
3. [[Basic with Staging & Data Marts]]

## Sizing
![[Pasted image 20231017002128.png]]

## Best Practices
1. Defining goals & objectives (Business alignment)
	- What can we derive out of this in terms of [[Business Intelligence]]
	- Make sure it aligns with Business Needs
2. Data Modelling ([[Tabular Data Warehouse]], [[Star Schema]], [[Snowflake Schema]])
	- Picking suitable approaches
3. [[ETL]] Processes (sources, mapping, refresh)
	- Sources = How do we bring data into [[Data Warehouse]]
	- Mapping = Transformation/Business Logic
	- Refresh = When do I add into [[Data Warehouse]]
4. Security, Scalability & Performance
	- Security = Data Marts, Backup
	- Scalability = How your [[Dimension]] table don't grow too much
	- Performance = How fast can you load, How fast can you do your refresh

<aside> 💡 Different approaches you take to move data to the point you can source & transform it </aside>
