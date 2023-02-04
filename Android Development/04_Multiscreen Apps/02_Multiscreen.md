#### Arrays

- **Create and Use an Array**
	- Create Array
	```Java
	int [] shoeSizesAvailable = new int[3];
	```
	- Initialize elements in an array
	```Java
	showSizesAvailable[0] = 5;
	showSizesAvailable[1] = 7;
	showSizesAvailable[2] = 10;
	```
	- Access elements in an array
	```Java
	shoeSizesAvailable[0] //Value of 5
	shoeSizesAvailable[1] //Value of 7
	shoeSizesAvailable[2] //Value of 10
	```
- Get the Array Length
	```Java
	shoeSizesAvailable.length // Value of 3
	```

- **ArrayList**
	- An array has a fixed length and hence it is limited when we want to add more values of the array data type and also in case of less values there are blank spaces in the array.
	- So we will be making use of ArrayList which can basically store object data types.
	- Now in order to store primitive data types like int, String, etc. we will be making use of Object Wrappers.
	- It wraps the primitive objects to convert them into an integer. 
	- For example ArrayList<Integer>, ArrayList<int>.
	- ![[Array vs Array List.png]] 
	- ![[Array vs ArrayList_2.png]]
	- ArrayList extends AbstractList. An abstractList is partially implemented, it has some methods implemented and some methods not implemented.
	- An AbstractList implements List. A List is a collection which maintains an ordering for its elements.
	- ![[Different Types of Classes.png]] 
	- ![[ArrayList.png]]
	- ArrayList: https://beginnersbook.com/2013/12/java-arraylist/
	
	
