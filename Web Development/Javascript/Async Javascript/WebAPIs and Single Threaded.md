## Web APIs and Single Threaded
---
### Notes
- Javascript at once is atmost learning one line of code, therefore it is single threaded.
- Therefore Javascript can run only one line of code at at a time. BUT....
- In cases of setTimeout where we used to console.log after a delay, for example
	```Javascript
	console.log("Sending request to the server");
	setTimeout(()=>{
	console.log("Here is your data from the server....");
	},3000)
	console.log("I am at the end of the file");
	```
- In cases like this, Javascript must actually stop running the code after the setTimeout as it is single threaded but instead the first console.log will be executed first and then the third console.log would be executed.
- Javascript actually gives the task to the browser to handle such tasks as the browser is written in languages such as C++ or Java which can handle multiple statements at once.
- The same happens in case of forms as well, see the pdf for detail.
- In the above code snippet, the task of setTimeout (or forms as well) are being passed to the Web API, the Javascript runs first and third console.log, after three seconds, browser reminds Javascript to run second console.log and then that is executed by Javascript itself.