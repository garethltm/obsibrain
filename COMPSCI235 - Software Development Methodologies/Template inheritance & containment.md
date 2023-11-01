![[Pasted image 20231101233731.png]]
- [[Template inheritance]]
- [[Template containment]]

Template can declare content blocks
- `{% block name %}...{% endblock %}`
[[Template inheritance]] is facilitated by the extends declaration
- `{% extends name %}`
	- Sub-templates inherits the structure, content blocks & expressions of their super-template
	- Sub-templates can override inherited content blocks & provide their own content
	- Sub-templates can inherit & extend inherited content blocks via the `super()` declaration
[[Template containment]] is provided by the include declaration
- {% inclu}