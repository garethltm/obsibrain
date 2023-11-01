[[transaction(s)]] are [[ACID]] compliant.
- **A**tomic - "all or nothing"
	- all actions in the [[transaction(s)]] happen or none happen
- **C**onsistent - "looks correct" - no in valid data
	- if each [[transaction(s)]] is consistent & the [[COMPSCI235 - Software Development Methodologies/database|database]] starts consistent, then it ends up consistent
- **I**solated - "as if alone" - 2 customers cannot book the same seat at the same time
	- execution of 1 [[transaction(s)]] is isolated from that of other transaction
- **D**urable - "survive failures"
	- if a [[transaction(s)]] commits, its effects persist