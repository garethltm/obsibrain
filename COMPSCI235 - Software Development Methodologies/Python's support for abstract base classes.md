![[Pasted image 20231102005437.png]]
- Python's `abc` module provides infrastructure for defining abstract classes
- To use `abc` (Abstract Base Class)
	- Make `AbstractRepository` a subclass of ABC
	- Tag all methods that `AbstractRepository` subclasses must implement with `@abstractmethod`
- At run-time, any attempt to instantiate a subclass of `AbstractRepository` that fails to implement an `@abstractmethod` results in a `TypeError exception`
- Using typing hints, anywhere an `AbstractRepository` is expected, an instance of a `AbstractRepository` subclass can be given