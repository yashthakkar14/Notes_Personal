## Position

Reference : ![[Other Useful CSS Properties#^position]]

---
### Different types of Position
- static
	- Default position for an element.
	- Properties like top, bottom, bottom-left,etc. have no effect on the position static.
- relative
	- Keeps the element in normal flow of the document.
	- But we can offset it relative to itself, using top,right,bottom,left.
- absolute
	- Element is removed from the normal document flow and no space is created for the element in the page layout.
	- It is positioned to its **closest positioned ancestor if any**: otherwise it is placed relative to the **initial containing block**.(in the example case, initial containing block is body)
	- **Position ancestor** is the ancestor which has its position set to anything other than static.
	- It's final position is determined by the values of top, right, bottom and left.
	- For example, if left is 1 px, then it is positioned 1 px to the left of ancestor
- fixed
	- Element is removed from the normal document flow and no space is created for the element in the page layout.
	- The position for that element will stay fixed to the top or to the position given in the offset.
- sticky
	- stays in it's original position until it hits the top, and then sticks to it.
	- it is similar to fixed but it is not fixed initially and gets fixed later.
		- Stays in its position
		- It begins not from the top position or the offset position but starts at its own position and then gets fixed later.
		- Refer MDN for the sticky docs.
---

### Tags
#Other_CSS , #node #position
