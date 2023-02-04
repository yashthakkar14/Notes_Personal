## CSS Units
---
### Types of Units
- Relative
	- EM
		- Refer Lecture and PDF - [[1.3 WDB CSS Box Model.pdf]]
		- With font-size, 1 em equals the font-size of the parent. 2em's is twice the font size of the parent.
		- With other properties such as padding, margin, 1em is equal to the computed font-size of the element itself.
			- For example, if an element is inheriting it's font-size from parent, say parent is 20 px and element's font-size is 5em's, then the property's 1 em will be equal to element's size, that is 5em's of parent element that is 100px.
		- We can give flexible rounded corners to an element using 0.5 em. The corners will stay rounded, even when the original image's font size changes. 
	- REM
		- Rem's are used to overcome the drawbacks of em's.
		- The drawback of em is when the elements are nested to each other like
		```HTML
			<ul>
				<li> Purple 
					<ul>
						<li> Pale Purple </li>
						<li> Orchid Purple </li>
						<li> Mauve Purple </li>
					</ul>
				</li>
				
				<li> Red
					<ul>
						<li>Crimson Red</li>
						<li>Fuchsia Red</li>
						<li>Maroon Red</li>
					</ul>
				</li>
				<li> Blue 
						<ul>
							<li> Turquoise Blue </li>
							<li> Powder Blue </li>
							<li> Sky Blue </li>
						</ul>
				</li>
			</ul>
			```
		- When we change the value of ul in em's with respect to parent element, the ul's stack and each ul increases in size of given em than the previous ul.
		- Rem's (Root Em's ) are relative to the root element's (HTML) font-size and not of parent's. They are often easier to work with.
		- If the root font-size is 20px, 1 rem is always 20 px, 2 rem is always 40px, etc.
		- You can change root default font-sizre by changing HTML font-size.
	- VH
	- VW
	- %
		- Always relative to some other value
		- Sometimes its value from the parent and other times it's a value from the element itself.
		- Examples :
			- width : 50% - half the width of the parent
			- line-height : 50% - half the width of the element itself.
	- AND MORE !
- Absolute
	- PX (Most commonly used in Absolute)
	- PT
	- CM
	- IN
	- MM
---

### Tags
#box_model , #node 
