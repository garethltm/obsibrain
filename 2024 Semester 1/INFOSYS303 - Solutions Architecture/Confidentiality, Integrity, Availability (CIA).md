![[Pasted image 20240527235958.png]]
### Three pillars of security: the [[Confidentiality, Integrity, Availability (CIA)]] Triad
- Confidentiality: information & functions can be accessed only by properly authorized parties
- Integrity: information & functions can be added, altered or removed only by authorized persons & means
- Availability: systems, functions & data must be available on-demand according to any agreed-upon parameters regarding levels of service
Security in IT essentially the protection of information, where information is represented in data
- information $\ne$ data
	- information, meaning of that data
	- data is what we manipulate
## [[Confidentiality, Integrity, Availability (CIA)]]
The NIST standard FIPS 199 characterizes [[Confidentiality, Integrity, Availability (CIA)]] in terms of requirements & the definition of a loss of security in each category as:
1. Confidentiality $\rightarrow$ Preserving authorized restrictions on information access & disclosure, including the means for protecting personal privacy & proprietary information. 
	- A loss of confidentiality is the unauthorized disclosure of information
2. Integrity $\rightarrow$ Guarding against improper information modification or destruction, including ensuring information nonrepudiation & authenticity.
	- A loss of integrity is the unauthorized modification or destruction of information
3. Availability $\rightarrow$ Ensuring timely & reliable access to & use of information.
	- A loss of availability is the disruption of access to or use of information or an information system
##### ++
4. Authenticity $\rightarrow$ The property of being genuine & being able to be verified & trusted; confidence in the validity of a transmission, a message or message originator. This means verifying that users are who they say they are & that each input arriving at the system came from a trusted source.
5. Accountability $\rightarrow$ The security goal that generates the requirement for actions of an entity to be traced uniquely to that entity. This supports nonrepudiation (basically showing who sent what as proof), deterrence, fault isolation, intrusion detection & prevention & after-action recovery & legal action. Because truly secure systems are not yet an achievable goal, we must be able to trace a security breach to a responsible party. Systems must keep records of their activities to permit later forensic analysis to trace security breaches or to aid in transaction disputes