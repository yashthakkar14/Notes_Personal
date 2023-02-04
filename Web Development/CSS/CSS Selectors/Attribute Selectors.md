## Attribute Selectors
---
Reference
![[CSS Selectors#^attribute]]

---
### Types of Attribute Selectors

1. CSS\[attribute\] selector
	- The \[attribute\] selector is used to **select elements with a specified attribute.**
	- The following example selects all \<a\> elements with a target attribute:
		```CSS
		a\[target\] { background-color: yellow;}
		```

2. CSS \[attribute = "value"\] Selector
	- This attribute is used to **select elements with a specified attribute and a value.**
	- Example : Selects all \<a\> elements with target="\_blank" attribute.
		```CSS
		a[target = "_blank"]{
			background-color : yellow;
		}
		```
		
3. CSS \[attribute ~= "value"\] Selector
	- This attribute is used to select elements with an attribute value **containing a specified word.**
	- The following example selects all elements with a title attribute that contains a **space-separated** list of words, one of which is "flower":
		```CSS
		[title~="flower"] {
			border: 5px solid yellow;
		}
		```
		
4. CSS \[attribute|="value"\] Selector
	- The \[attribute|="value"\] selector is used to select elements with the specified attribute **starting with the specified value.**
	- The following example selects all elements with a class attribute value that begins with "top":
	- **Note:** The value has to be a whole word, either alone, like class="top", or followed by a hyphen( - ), like class="top-text"!
		```CSS
		[class|="top"] { background: yellow;}
		```
		
5. CSS \[attribute^="value"\] Selector
	- The \[attribute^="value"\] selector is used to select elements whose attribute value begins with a specified value.
	- The following example selects all elements with a class attribute value that begins with "top":
	- **Note:** The value does not have to be a whole word!
		```CSS
		[class^="top"] { background: yellow;}
		```
		
6. CSS \[attribute$="value"\] selector
	- The \[attribute$="value"\] selector is used to select elements whose attribute value ends with a specified value.
	- The following example selects all elements with a class attribute value that ends with "test":
	- **Note:** The value does not have to be a whole word!
		```CSS
		\[class$="test"\] { background: yellow;}
		```
		
7. CSS \[attribute*="value"\] selector
	- The \[attribute*="value"\] selector selector is used to select elements whose attribute value contains a specified value.
	- The following example selects all elements with a class attribute value that contains "te":
	- **Note:** The value does not have to be a whole word!
		```CSS
		\[class\*="te"\] { background: yellow;}
		```

---
### Tags
#selectors #node 

---