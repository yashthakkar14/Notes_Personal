## Box Model Width,Height and Border
---
### Height and Width
- Used to control the width and the height of the specified element.
- Width is taken as x-axis whereas height as y-axis.
- Works only in block level elements and doesn't work in inline.
---
### Border
- Border Properties
	- border ( Provide in order width | style | color - shorthand property)	
	- border-width
	- border-color
	- border-style
		- [[Border-Style Properties.png]]
	- border-left-style
	- border-left-color
- Border-box
	- It allows us to include the padding and border in element's total width and height.
	- When an element is given a  specific size, for example, let's say 200px.
	- Then the content of the element without border would be 200 px.
	- However, if border-box is given, 200 px will be subtracted from the border if any and the inner content size would be from remaining px.
	- Synax
		```CSS
		.square{
		box-sizing:border-box
		}
		```
- Border-radius
	- Use to create elliptical, circular, rounded or border-shape elements.
	- Example : border-radius : 50 %

---
### Tags
#box_model #node 

---