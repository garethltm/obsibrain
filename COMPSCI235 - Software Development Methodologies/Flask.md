- [[Flask]] is a Web application (web-based [[Middleware]]) framework
	- collection of packages & modules
	- simplifies development of Web applications

- [[Flask]] is 1 of 2 widely used Web application frameworks for Python
	- Django is a more established framework that is more complex, comprehensive & suited to experienced developers
	- [[Flask]] has been developed to be as simple as possible, allowing for extensions to be used where required
		- lightweight & easy to use![[Pasted image 20231101231147.png]]![[Pasted image 20231101231220.png]]

### `route()` decorator & views
- `route()` decorator is used to bind a function (a view) to a URL
- `route(rules, options)`:
	- rule - URL binding with the function
	- list of parameters to be forwarded to the Rule object
- allows to add variable sections to URL using angled brackets '<>'.

### `app.run()`
- [[Flask]] application gets started by calling run() method.
- app.run(host, port, options)
	- host - hostname to listen on (default - 127.0.0.1 (localhost))
	- port - (default - 5000)