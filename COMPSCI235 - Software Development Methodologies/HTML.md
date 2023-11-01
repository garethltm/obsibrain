- used to format web pages
- contains hypertext information (links)
- written in ASCII/Unicode
- embedded format codes (tags)
![[Pasted image 20231101161908.png]]

### Document Type
defines which standard is being used for the page
- we use HTML5

`<!DOCTYPE html>`
- this should appear at the top of the file

### Encoding methods
different character sets used to encode the page
- ASCII
- UTF-8
- Unicode
Need to tell the browser which encoding is used

`<meta charset="UTF-8">`
- located in the `<HEAD>` of the document

# Tags
Elements are the building blocks of web pages
- Designators that define the content & the structure of objects in a page

Markup achieved with "tags"
- enclosed with angle brackets `<...>`
- use lower case

![[Pasted image 20231101162122.png]]

### Attributes
some tags require additional information
- properties or attributes of the tag
`<tag property = "value"></tag>`

## Nested Tags
tags must be correctly nested
- cannot close an open tag until all the open tags that it affects are also closed
![[Pasted image 20231101162311.png]]

## Essential Tags
1. `<html lang="en">`
	- encloses the entire document
	- specifies that the document uses `html`
	- `lang` attribute is used to specify the primary language of a webpage
		- `en` is the code for English
![[Pasted image 20231101162504.png]]
2. `<head>`
	- doesn't contain any content to be displayed on the page	
	- contains information for the browser
	>	#Example 
	>	character encoding used
![[Pasted image 20231101162635.png]]

3. `<body>`
	- contains all the content that will appear on the page
![[Pasted image 20231101162926.png]]

4. `<title>`
	- part of the `head`
	- specifies the title to be used by the browser
	- name of the window
	- used in navigation
	>	#Example 
	>	bookmarks, history, etc.
![[Pasted image 20231101163110.png]]

# Block-level tags
![[Pasted image 20231101163215.png]]
define the structure of a "block"
- #### Paragraphs `<p>`
	- defines a paragraph of text![[Pasted image 20231101163424.png]]

- #### Headings `<h1>,<h2>,<h3>,<h4>,<h5>,<h6>`![[Pasted image 20231101163552.png]]
	- 6 levels of headings![[Pasted image 20231101163627.png]]
- #### Lists
	1. Ordered Lists 
	- automatically numbered
		`<ol>`
		- contains the entire list
		`<li>`
		- used for each list item![[Pasted image 20231101164037.png]]
	2. Unordered Lists
	- bullet points
		`<ul>`
		- contains the entire list
		`<li>`
		- used for each list item![[Pasted image 20231101164211.png]]
	3. Description Lists
	- terms & explanations
		`<dl>`
		- contains the entire list
		`<dt>`
		- defines a term in a description list
		`<dd>`	
		- is used to describe a term in a description list![[Pasted image 20231101164411.png]]
- #### Tables `<table>`
	- used to format tables of information
	- by default, there are no borders shown
	- ###### Tags
		`<table>`
		- surrounds the entire table
		`<tr>`
		- identifies a row in the table
		`<th>`
		- each heading in the header row
		`<td>`
		- each element/cell of data in the 
