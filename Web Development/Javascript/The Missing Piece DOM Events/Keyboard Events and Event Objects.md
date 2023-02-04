## Keyboard Events and Event Objects
---
### Event Objects
- Event objects are automatically passed in to the function (or callback).
- We can name it whatever we want but usually it is called event or e or evt.
- Client X and Client Y are the co-ordinates which are relative to the window where you type.
- We need to rely on event objects when using keyboard events because we particularly need to know which key was pressed.
- Syntax
	```Javascript
	const input = document.querySelector("input");
	input.addEventListener("keydown",(e)=>{
	console.log(e);
	console.log(e.key);
	console.log(e.code);
	})
	```
---
### Keyboard Events
- Keyboard events helps us know which key was pressed or in general events related to the keyboard.
- Particularly out of many information given in the keyboardEvent object, key and code are important.
- key gives us the actual key we pressed.
- code gives the location of it on keyboard.
- So you can also change the language and the key will give information of what is actually typed whereas code will tell what key was actually typed on keyboard.
- For example फ will show फ in key but it will show keyH in code.
- Code is mostly used in cases of when a game is made like when we need wasd where they key pressed is of importance but if we want actual letters then we can use key instead of code.
- You can use keyboard events for a specific element or for the whole window. For a specific element, you can choose using query selector or you can use window object for the whole window.
- Example
	```Javascript
	window.addEventListener('keydown',e=>{
	 switch(e.code){
	 case 'ArrowUp':
	 console.log("UP !");
	 break;
	 case 'ArrowDown':
	 console.log("DOWN !");
	 break;
	 case 'ArrowLeft':
	 console.log("LEFT !");
	 break;
	 case 'ArrowRight':
	 console.log("RIGHT !");
	 break;
	 default:
	 console.log("IGNORED");
	 }
	})
	```
---