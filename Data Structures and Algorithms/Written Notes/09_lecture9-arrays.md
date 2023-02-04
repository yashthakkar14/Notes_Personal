## Arrays

- Should have similar type of item. (only int, char, bool, float, double, etc.)
- Values are stored in contiguous memory location. (Written Notes for more info...)
- Elements of the array can be accessed with the help of an index.
- An array is needed to store multiple same type of values.
- **Declaration** : Declaring an array `int arr[10];` 
- arr is the name of the array as well as it also signifies the location of the first integer present in the array.
  - That is when you simply print out arr, `cout << arr;`. You'll get the address of the first element of the array.
  - Refer to the **09_01_int-arrays.cpp** program file's 1st program. The address of the array and the address of the first element of the array is printed which is exactly the same, therefore the array also signifies the address of the first element of the array.
  - Also the address of the second element of the array is 4 bytes ahead of the address of the first element of the array which further signifies that the array is contiguous as it takes 4 bytes to store an integer.
- The values in the array will be initialized with the garbage value.
  - Refer to the program referred above again.
- If array is of size n, the index of the array will range from 0 to n-1.
- **Accessing** : The elements can be accessed as arr[0], arr[1], .... arr[n-1] where arr[0] represents 1st element of the array and arr[n-1] represents last element of the array.
- **Initializing the array** : int number[3] = {5,7,11};
  - Here number[0] = 5, number[1] = 7, number[2] = 11.
  - number[3] = {0}. All the values will be initialized with 0.
  - The above expression can work just in the case of 0 and not with any other integer.
  - For e.g. number[3] = {1} will not set all the values of the number to 1, it will initialize the first value of the number array to 1 and rest all the elements in the number array will be equal to 0. 
  - In order to initialize all the elements in an array with some value other than 0, we can use two approaches.
    1. The first one is where we access each element of the array using for loop, we specify the end of the for loop using 
    sizeof(arr)/sizeof(arr[0]) which specifies the total size of the array divided by the size of the first element of the array. We know that the size of the array is equal to the sum of size of all the elements present in the array and we divide it by the size of the single element in the array so as to know the number of elements present in that particular array. 
    2. The second method is to use the fill and fill_n method. The fill method contains the start address, the end address and the value to initialize. The fill_n method contains the start address, the no. of elements to fill and the value.