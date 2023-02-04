## Combinator Selectors
---
Reference 
![[CSS Selectors#^combinator]]
- Example data
	- Example
		```HTML
		<div>
		<p> Paragraph 1 in the div </p>
		<p> Paragraph 2 in the div </p>
		<section><p> Paragraph 3 in the div </p></section>
		</div>
		<p> Paragraph 4 after the div </p>
		<p> Paragraph 5 after the div </p>
		<div></div>
		<section><p>Paragraph 6 after the div but in the section</section> 	
		<p>Paragraph 7</p>
		``` 

---
### Types of Cominator Selectors
1. Descendant Selector
	- Matches all the elements that are descendants of a specified element
	- Example : Select all  p's that are nested inside a div
	- This will color all the paragraphs which are present inside the div, in this case **paragraphs
		 1, 2 and 3**
		```CSS
		div p{
			color : teal;
		}
		```
2. Adjacent Sibling Selector (+)
	- Used to select an element that is immediately after another specified element.
	- Example : Selects only the paragraphs that are immediately preceded by a div.
	- This will color all the paragraphs immediately after any div element, in this case, it will color **paragraph 4** (It won't color paragraph 6 because it is nested inside a section and not 7 too as it is not immediately after the div element.)
		```CSS
		div+p{
		color:red;
		}
		```
3. Direct Child(or Descendant) Selector (>)
	- The child selector selects all the elements that are the children of a specified element.
	- Example : Selects only the paragraphs that are direct child of the div element.
	- This will color all the paragraphs which are direct child of div element, in this case, **paragraphs 1 and 2.**
		```CSS
			div>p{
			color:red;
			}
			```
4. General Sibling Selector (~)
	- The general sibling selector selects all the elements that are siblings of the specified element 
	- Example : Select all the paragraphs that are siblings of div elements.
	- This will color all the paragraphs which are siblings of div element, that is all the paragraphs after div element, in this case **paragraphs 4,5 and 7.**
		```CSS
		div~p{
			color:purple;
			}
		```

---
### Tags
#selectors #node 

---
	
	
