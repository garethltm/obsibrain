any action you need to do to convert your resources (images,etc.) to build your final product
- what are the steps we need to build the code

not using a virtual environment to install [[software dependency]]

Python:
- `PyBuilder`
	- A Python package with a `pyb` command
	- `build.py` code the [[build scripts]] in Python
	- Can be integrated as a plugin into PyCharm

Java:
- `Ant/Gradle/Maven`
	- Create `build.xml` for a project (a Java `Makefile`)
		- Type command `ant` in the project folder

C++:
- `CMake`

Building tasks in motion, from building [[software]] to deploying it
![[Pasted image 20231103120001.png]]

### Ultimate goal:
- Anyone should be able to bring in a virgin machine, check out the source code & other necessary resources from the repository, ideally issue a single command & have a running [[software]] package on their machine
	- no need of using an IDE to run your application