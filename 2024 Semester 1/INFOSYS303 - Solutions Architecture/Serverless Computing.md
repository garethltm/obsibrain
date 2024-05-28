- is a [[Cloud Computing]] execution model in which the cloud provider allocates machine resources on demand, taking care of the servers on behalf of their customers
- developers of serverless applications are not concerned with:
	- capacity planning
	- configuration
	- management
	- maintenance
	- [[fault-tolerance]]
	- [[2024 Semester 1/INFOSYS303 - Solutions Architecture/Scalability|Scalability]]
		of VMs or physical servers
When an app is not in use, there are no computing resources allocated to the app. Pricing is based on the actual amount of resources consumed by an application. [[Serverless Computing]] is a form of utility computing
## Advantages
#### Cost
- Serverless can be more cost-effective than renting or purchasing a fixed quantity of servers, which generally involves significant periods of underutilization or idle time
	- can be described as a pay-as-you-go computing or bare-code as users are charged based solely upon the time & memory allocated to run the code without associated fees for idle time
	- Immediate cost benefits are related to lack of operating costs, including: licenses, installation, dependencies & personnel cost for maintenance, support or patching
#### Elasticity vs [[2024 Semester 1/INFOSYS303 - Solutions Architecture/Scalability|Scalability]]
- A serverless architecture means that developers & operators do not need to spend time setting up & tuning autoscaling policies or systems
	- the cloud provider is responsible for scaling the capacity to the demand
- As cloud native systems inherently scale
## Major providers
- Google App Engine, introduced in 2008 was the first abstract [[Serverless Computing]] offering.
	- It was used to support early customers including Snapchat, as well as many external & internal Google apps.
	- Google App Engine used pay-for-what-you-use billing
- AWS Lambda, introduced by Amazon in 2014
	- it popularized the abstract [[Serverless Computing]] model
	- It is supported by AWS Serverless Application Model (AWS SAM)
- Google Cloud Platform created a second serverless offering, Google Cloud Functions in 2016
- Oracle Cloud Functions is a serverless platform offered on Oracle Cloud Infrastructure
	- Since it is open-source, developers can create applications that can be ported to other cloud & on-premise environments.