1. allows you to conveniently code unit tests using Python's `assert` statement
	- the approach in [[Pytest]] is to write test cases that cause can object to change its state, and then assert that the object's actual state matches with what's expected

2. provides the means to run a [[test suite]] & view the results

3. relies on naming conventions to discover tests
	- [[test suite]]
	- an individual test is implemented as a function whose name begins with `test_`

### [[Pytest]] fixtures
- good for writing multiple tests
- [[Pytest]] provides the fixture decorator that can be used to supply tests with a freshly initialised object to test
