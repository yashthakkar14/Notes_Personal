1. An array is a collection of items of similar type stored in contiguous memory locations.
   1. Whenever we declare an array, for example `int arr[5];`.
   2. This means two things, one being that the name of the array is 'arr'.
   3. And the second being that, arr points to the first address of the first element of the array.
2. Arrays and pointers
![](09_arrays_pointers.png)
3. What happens in pointers is we declare a variable and then if we prefix '&', for e.g &a, then we can get the address of variable a.
4. However in arrays, it is different case, here the name of the array itself is the address of the first block of array.
5. Initialising entire array with a single value 
https://www.techiedelight.com/initialize-elements-array-same-value-c-cpp/#:~:text=Using%20Initializer%20List&text=int%20arr%5B%5D%20%3D%20%7B%201,0%20in%20the%20initializer%20list.
6. sizeof() operator
   1. The sizeof() operator in case of an array returns the size of an array.
   2. That is, if we have an array, the sizeof() operator will return the length of the array multiplied by the size of the datatype stored in that particular array.
   3. So in order to find the length of the array, we need to divide the size of the array by the size of the datatype.
   4. For example
        ```
        int arr[5] = {1,2,3,4,5};
        int arr_len = sizeof(arr)/sizeof(arr[0]);
        ```
7. ARRAYS WITH FUNCTIONS
   1. We can also pass array to a function as shown in the code [09_01_arrays - line 6].
   2. When passing array to a function, you need to pass two things, one is the array and second in the length of the array.
   3. The length of the array can be calculated using sizeof() operator as shown in point 6 above and then passed to the function as shown in the code.
8. Similarly we can have array of characters, double, float, boolean.
9. Having a variable passed into the array as size is a really bad practice.
   1. For example, having n as a variable which is initialized or asked from the user.
   2. If we pass 'n' as the size of the array as arr[n], it is considered as a bad practice.
   3. Instead of that, we can define an array size by default like 10000 or any other large value even if we are going to store less values init.
   4. When to use variable will be seen when using pointers.
10. INT_MIN and INT_MAX
   1. Integer has a range -2^31 to 2^31-1.
   2. Here the INT_MIN is -2^31 and INT_MAX is 2^31-1
11. Passing array to a function and then updating it.
    1.  In case of variable, we studied that when we pass a variable to a function and then update the variable, the original variable is not updated and the function variable is updated.
    2.  This was because the function creates a copy of the variable which we passed to the function
    3.  However, this is not the same with arrays.
    4.  When we pass array to a function, we are actually passing the address to the function as the name of the array points to the location of the first element of the array.
    5.  That is, we are not passing the value of the elements of the array or the array in itself is not copied to the function, but instead we are passing the address of the actual array to the function.
    6.  So whatever changes the function makes is done on the original array itself.
    7. In case of integer, we used to pass the value of the integer to the function and the function used to create a separate memory block and then stored that value.