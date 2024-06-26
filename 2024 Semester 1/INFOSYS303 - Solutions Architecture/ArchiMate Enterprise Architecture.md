- An [[Enterprise Architecture]] is a response to concerns by "stakeholders" that need to be addressed by the business & IT systems within an organization
- The role of the architect is to address these concerns by:
	- identifying & refining the motivation & strategy expressed by stakeholders
	- developing an architecture
	- creating views of the architecture that show how it **addresses & balances stakeholders concerns**
		- proving a case to the stakeholders

The [[ArchiMate Enterprise Architecture]] modeling language provides a uniform representation for diagrams that describe [[Enterprise Architecture]]

It includes concepts for specifying
- inter-related architectures
- specific viewpoints for selected stakeholders
- language customization mechanisms
(expressing our ideas in a graphical form that is easy to understand)

The language uses service-orientation to distinguish & relate the Business Application & Technology Layers of [[Enterprise Architecture]] & uses realization relationships to create concrete elements to more abstract elements across these layers

### Top-level hierarchical structure of the language
- A model is a collection of concepts
	- a concept is either an element or a relationship
- An element is either:
	- a behavior element
	- a structure element
	- a motivation element
	- a composite element
![[Pasted image 20240318001649.png]]

## Layering of the ArchiMate Language
The [[ArchiMate]] core language defines a structure of generic elements & their relationships which can be specialized in different layers

3 layers are defined within the [[ArchiMate]] core language as follows:
1. The Business Layer depicts business services offered to customers, which are realized in the organization by business processes performed by business actors
2. The Application Layer depicts application services that support the business & the applications that realize them
3. The Technology Layer comprises both information & operational technology

We can model, for example:
1. processing, storage, communication technology
	in support of the application world & Business Layers
2. model operational or physical technology 
	with facilities, physical equipment, materials & distribution networks

The general structure of models within the different layers is similar. The same types of elements & relationships are used, although their exact nature & granularity differ
- In alignment with service-orientation, the most important relationship between layers is formed by "serving" relationships, which show how the elements in one layer are served by the services of other layers
- A second type of link is formed by realization relationships: elements in lower layers may realize comparable elements in higher layers