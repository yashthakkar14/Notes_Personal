## Events and the Keyword This
---
### Notes
- When you are acting on multiple buttons or h1's together For e.g
	```Javascript
	const buttons = document.querySelectorAll(button)
	for(let button of buttons){
	button.addEventListener(click,function(){
	button.style.backgroundColor = makeRandColor();
	})
	}
	const h1s = document.querySelectorAll(h1)
	for(let h1 of h1s){
	h1.addEventListener(click,function(){
	h1.style.color = makeRandColor();
	})
	}
	```
- Here if you want to create a new colorize function, it is not possible to reference to the exact same button.
- This is when the keyword 'this' is helpful.
- 'this' helps us to refer to whatever was clicked on that triggered the function.