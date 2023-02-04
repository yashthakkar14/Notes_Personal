### Java Basics

- Variable naming conventions.
    - Variable names are case sensitive.
    - Variables follow camel case notation.
    - Start variable names with a letter.
    - Cannot have white spaces.
- String variables
    - variable.length() - length of the string.
    - variable.toUpperCase() - convert every letter of the string to a capital letter.
    - variable.toLowerCase() - convert every letter of the string to a lowercase letter.
    - String concatenation (+).
- Variable types (numbers)
    - Integer (Number)
        - int maxInt = 1234567890
        - limited to 10 digits.
    - Long (Number)
        - Can create much larger numbers.
        - At the cost of extra space.
    - Double (Number)
        - Can store fractional numbers.
        - Extra space.
        - double div = 5/2
        - The above value would be 2 even though we are storing it in double as we are dividing two integers.
        - Make sure that one  of the numbers is double to get accurate result for e.g 5/2.0
    - String (Text)
        - Can store string.
        - Wrapped with double quotes.
    - Character (Text)
        - Can store single letter.
        - Wrapped with single quotes.
        - char three ='3'.
    - Boolean
        - boolean fact = true.
- Casting and comments.
	```Java
	double current = 17;
	//current will be stored as 17.0
	double rate = 1.5;
	double future = current * rate;
	System.out.println(future); //casting
	int approx = (int)future;

	/*
	This is a
	comment
	*/
	```

---

