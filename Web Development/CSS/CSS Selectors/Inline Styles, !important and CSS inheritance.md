### Inline Styles
---
- Inline styles are **more specific than IDs and Elements and Classes.**
- They are the most specific thing yet.
- Inline style is the style in HTML given as an attribute in the tag.
- It is recommended to **avoid the inline styles** as they are even seperate from the CSS stylesheet.
- Example
	```CSS
	<button id = "signup" style = "color:coral">Sign Up </button>
	```
- Among inline(style attribute), internal(style tag) and external stylesheet the order of priority is 
  inline  > internal > external
---

### !important exception
- The !important exception overrides all the styles including inline styles and id, class and element selectors.
---
### CSS Inheritance
- The child elements in most cases inherit properties from the parent elements if no CSS property is given explicitly to the child element.
- This concept is known as CSS inheritance.
- If a child element is given styles and later a parent element is given styles, then the parent element will not override child styles as the child is more specific.
- Not all elements inherit directly from the parent, unless explicitly mentioned, for example input and button.
- Not all properties are inherited (for example border)
---

### Tags
#node, #selectors 

---