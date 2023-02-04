### Function Basics

- Example
    ```Java
    public void chorus(){
    //print out 4 lines of chorus
    System.out.println("Once I had a love and it was gas");
    System.out.println("Soon turned out had a heart of glass");
    System.out.println("Seemed like the real thing, only to find");
    System.out.println("Mucho mistrust, love's gone behind");
    }
    ```
- Let's understand this code
  - public
    - access modifier.
    - anyone can use public functions.
  - void
    - return type
    - not returning any data
  - chorus()
    - function name
    - how we call our function

### Function Parameters and Arguments

- Parameters - Variables in the parentheses of our function that we can then use inside our function.
- Example
    ```java
    public void greeting(String location){ //parameter
    //greet a specific location
    System.out.println("Hello, " + location);
    }
    greeting("Kalyan Super Smart City"); //argument
    ```
    
- Multiple parameters example
    ```java
    public void printPhoto(int width, int height, boolean inColor){
    System.out.println("Width =" + width + "cm");
    System.out.println("" =" + width + "cm");
    ```