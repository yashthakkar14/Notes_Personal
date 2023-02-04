## Form Events & Prevent Default
---
### Prevent Default
- preventDefault Method helps us to prevent the default behaviour that happens due to the result of an event.
- For example submitting a form refreshes the current page or takes us to a new page.
- You cannot write Prevent Default in general but it is on the event object.
- Example
	```Javascript
	const submit_form = document.querySelector("#submit_form");
	submit_form.addEventListener('submit',function(e){
	e.preventDefault();
	 const p1 = document.createElement('p');
	 p1.innerHTML = "Hello ! How are you"
	 document.body.appendChild(p1);
	});
	```
---
### Form Events
- In Form, elements is a collection of all the form elements.
- You can select the form elements either by order or if a name is specified for a particular form element in the HTML form, we can directly use the same name as well.
- **Process of code :** 
- We first of all create a submit event which is triggered when a form is submitted.
- Then we use prevent default method on the event object to prevent the default action of sending data.
- Then we take the username and tweet value and create a list element in which we append bold tag and append username in the bold tag.
- Then we append new tweet to list and finally append the li item in the ul which was already created.
- Also one thing to note here, is that for selecting two inputs, we are making use of name and not the default index given by form.elements, so that we can select the distinct element.
- Example
	```Javascript
	const usernameInput = tweetForm.elements.username;
	const tweetInput = tweetForm.elements.tweet;
	 addTweet(usernameInput.value,tweetInput.value);
	 usernameInput.value = '';
	 tweetInput.value = '';
	```
- Here the 'elements' is an HTML form property which returns all the form controls contained in the \<form\> element.
- The addTweet function performs all the code explained before the code snippet and returns the tweet and the username and then we later clear the input fields.
---