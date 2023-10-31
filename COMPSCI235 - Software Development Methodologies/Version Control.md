## Why Version Control



## Version Control Systems (VCS)
- Also known as source code management systems or revision control systems
- A system that records changes to a data file or set of data files over time so that one can recall and compare specific versions later

- Data can be:
    - text
    - webpage content
    - code (python, java, etc.)
    - etc.
- Example VCS are:
    - Git
    - Subversion (SVN)
    - Mercurial, etc.
- Software developers control and maintain not just source code but an **entire code base**
    
- Includes:
    
    - Source code
    - Documentation
    - Build tools (Makefiles etc.)
    - Configuration files
    - Media files
    - Others (which are required for build)
- Does not include:
    
    - Just one certain type of file
    - Compiled files or library files, virtual environments in Python
    
    <aside> 💡 **.git ignore** - is how we usually ignore those types of files
    
    </aside>
    

<aside> 💡 Olden days concept of local VCS: the idea of having one central server and people going to commit changes to that one central system

disadvantage: if that server dies down, you won’t have access to your repositories

</aside>
