"***Failure is inevitable***"

Each of the many [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] might fail 
- Services might have bugs
- Services might be slow to respond
- Entire servers might go down

**The more [[2023 Semester 2/COMPSCI235 - Software Development Methodologies/Microservices]] there are, the higher the likelihood at least one is currently failing (probability to fail is much larger)**

Key:
- design every service assuming that at some point, everything it depends on might disappear
	- must fail "gracefully"

>	#Example 
>	Netflix uses "ChaosMonkey"
>	- which is responsible for randomly terminating instances in production to ensure that engineers implement their services to be resilient to instance failures