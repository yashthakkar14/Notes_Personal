## Switch and Functions


### Switch
- What we are doing in the switch statement is that we are comparing the character or integer given in the switch expression to the cases.
- If any case matches the switch expression, then that particular case is executed.
- If in an infinite while loop with no break statement, if we need to exit from the switch loop, we can use the exit() function where exit(0) represents that the program ended successfully whereas exit(1) indicates that the program exit was abnormal or due to an error.
- Continue in case of switch is not valid.
- What happens in case of continue in for loop is that suppose if we have continue in for loop, then the continue will skip that particular iteration and carry on its operation for all the further iterations, if any.
- However, in case of switch statement, the switch statement will keep on continuing the switch statement which does not make any sense as it will go into an infinite loop.
- We can include constants in the switch statement and can also include expression which evaluates to be a constant in the switch statement.
- Homework Question : Total amount = 'x' rupees. How many 100, 50, 20, 1 notes will be needed for the rupees.

### Functions
- Problem having well defined task.
- Function syntax
    ```C++
    return_type functionName(arguments){
        return <something>
    }
    ```
- return type can be int/char/float/string.
- arguments are variables passed to the function and parameters are the variables which is a copy of arguments used by the function itself.
- Arguments and parameters are not same, they are different. Whenever a variable is getting updated in the function, it is the variable of the function which is being updated.
- The function creates a copy of arguments passed to it which is known as function parameters.
- In case of functions with void datatype, we can use `return ;` which signifies that it is returning no value but it is just returning the control back to the main function.
- Function stack. Already known, as explained in the javascript course and the DSA course as well.