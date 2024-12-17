The [[Flask]] framework provides blueprints as a means to organise application functionality into different units

A [[Flask Blueprint]] is analogous to a Python module (`browse.py`)
- The content of a blueprint (module) should be cohesive
- A blueprint (module) should have a [[Single Responsibility Principle (SRP)]]

Blueprints are registered with the [[Flask]] application object; requests are routed through the "right" blueprint
	![[Pasted image 20231102000044.png]]