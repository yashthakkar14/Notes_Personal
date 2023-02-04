#### Multiscreen Apps
- Main activity is the main screen of our app.
- mipmap is a special folder just for the app icon.
- You can think of activities as a single screen in our app.

#### AndroidManifest.xml file
- Every app must have an AndroidManifest.xml file.
- You can think of this file as a table of contents for your app.
- It summarizes the important information about the whole app in a single place.
- https://developer.android.com/guide/topics/manifest/manifest-intro

#### Intents
- An **intent** is a message that requests some type of action to be performed by another app.
- https://www.vogella.com/tutorials/AndroidIntent/article.html#usingintents_call
- Creating a new intent accepts two parameters.
	- One being the context.
	- The second is the class component.
	- We need .class in the end to identify the specific java class.
- **this** in the context refers to the current activity.
- The **context** helps the intent to know more about the current state of the app.
- **Types of intents**
	- **Implicit intent**
		- Create an implicit intent if you don't care which app component handles the intent as long as they can.
		- For e.g in JustJava app you just needed an email app to open no matter which app is opening.
		- ![[Implicit Intent.png]]
	- **Explicit intent**
		- Create an explicit intent if you know exactly which app component should handle your intent.
		- In explicit intent, we explicitly state what activity should open when an intent is given to the android system.
		- We should never use explicit intents to open a third party app as we can never guarantee that a third party app we intend to call is actually installed on the device. 
		- Therefore, explicit intents are used within the same application as the developer knows what activities area available.
		- ![[Explicit Intent.png]]
		- ![[Implicit and Explicit Intents.png]]

#### Event Listeners
- https://developer.android.com/reference/kotlin/android/view/View.OnClickListener?hl=en
- The onClick property accepts just one input which is the view being clicked on and have no return value.

#### Interfaces
- Interfaces have no state but it does contain method signatures.
- A method signature signifies the return value, method name and the input parameters, it ends with a semicolon and there are no curly braces and code for implementation of the method.
- This means that it is an abstract method.
- In abstract methods, implementation is intentionally left blank so that a developer who wants to use interface can provide their own specific instructions for it.
- ![[Interface and Classes.png]]

#### Event Listener
- An onClick method is an interface with an abstract method called onClick.
- ![[Setup Event Listener.png]]
- ![[Setup Event Listener 2.png]]
- ![[Setup Event Listener 3.png]]
- Here, the **implements** is a Java keyword that has a special meaning.
- We use the implements to express that the NumbersClickListener class will support the specified interface (here OnClickListener is the interface) and provide code for all its abstract method.
- Therefore in short, an **Event Listener has three steps:**
	- Define an Event Listener
	- Create a new instance object of the Listener.
	- Attach the listener to the view.
- https://titanwolf.org/Network/Articles/Article?AID=0071103a-6b4f-4b68-96f5-757b0c0f92c9
- ![[Create Object with Constructor.png]]
- Difference between OnClickListener and OnClick : 
https://classroom.udacity.com/courses/ud839/lessons/7633778648/concepts/08cc4ffc-853e-456a-9d92-c455c1b60c43