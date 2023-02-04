## Input and Change Events
---
### Change Event
- Change event is fired when there is a change in the input value. 
- **Note:** It only reflects back the changes when the input field is left by the user or the input filled is blurred, it then reflects whatever changes are made by the user in the input field.
- This is useful when we don't want to frequently update the changes in the input field live but rather we only want to change the input when the user is done adding the value in the input field.
- Example
	```Javascript
	const input = document.querySelector('input');	
	input.addEventListener('change',()=>{
	alert(input.value);
	})
	```
---
### Input Event
- Input event is triggered continuously on the go as the user keeps on changing the input. 
- Here, user leaving the input is not mattered because as the user keeps on typing the event is triggered simultaneously.
- Example
	```Javascript
	const input = document.querySelector('input');
	const h1 = document.querySelector('h1')
	input.addEventListener('input',()=>{
	 h1.innerText = input.value;
	})
	```