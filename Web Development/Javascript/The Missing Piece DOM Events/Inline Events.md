## Inline Events
---
- We can add an event and the code corresponding to it inline to an element.
- For e.g
	```HTML
	<body>
		<button onclick = "console.log('This is a code'); alert('Stop clicking me')">Click ME !!
		</button>
	</body>
	```
- Check the code to understand it better.
- This is not the preferred method for events and you must avoid this method.
- The reason is then for each and every button we need to have the recurring code and it is kind of janky to include Javascript in HTML.