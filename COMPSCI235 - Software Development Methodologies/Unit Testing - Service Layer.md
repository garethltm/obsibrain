The `service layer` can be unit-tested similarly to the domain model classes

The purpose of testing the service layer is to find any cases where `service layer` logic is not behaving as expected

`conftest.py`
- where fixture code is common to multiple test files, it should be refactored (extracted into `conftest.py`)
	- this returns a freshly initialized object

[[Pytest]] automatically loads the contents of `conftest.py` prior to running tests
- `test_domainmodel.py`