### Ways to include styles in CSS


- Inline Styles
	- You can write your styles directly inline on each element. 
	- **Not recommended.**
	- Inline Styles Syntax ^inlinestyles
		```HTML
		<h1 style = "color:red"> 
		 ```
	
- The Style Element
	- Include styles inside of a style element.
	- Impossible to share styles between documents.
	- **Not recommended.**
	- Style Element Syntax ^styleelement
		```HTML
		<style>
			h2{
				color:red;
			}
		</style>
		 ```
		 
- External Style sheet
	- Write styles in a CSS file.
	- Include it using <link> in the head of your html document.
	- **Recommended.**
	- External Style sheet Syntax ^external
		```HTML
		<link rel ="stylesheet" href = "css_file.css">
		``` 


### Tags
- #basics, #node