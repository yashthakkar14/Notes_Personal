**How to calculate running time**

1. The running time of an algorithm depends on the following factors
   1. Single vs multiple processors
   2. Read and write speed of an algorithm
   3. 32 bit vs 64 bit architecture
   4. Configuration of the machine
   5. **Input**
2. We need to evaluate time as a function of input.
3. 1 unit of time is taken for arithmetic (+,-,/,*) and logical (AND, OR, NOT, XOR) operations.
4. Also it takes 1 unit of time for assignment and return statements.
5. In order to find Big-O notation, we need to find the worst case possible of the given algorithm that is we need to find the highest possible time it may take for the algorithm to complete.
6. In case of a for loop which traverses from 0->n, the time complexity will be O(n) if and only if the code inside of the for loop is of constant time complexity that is O(1).

**Frequency count method**
1. The time taken by an algorithm can be known by assigning one unit of time for each statement.
2. If any statement is repeating for some number of time, the frequency of execution of that statement will be calculated and we will calculate the time taken by the algorithm.


**Notations**
1. Big-O Notation
   1. Upper Bound.
   2. Worst Case Complexity.
2. Omega Notation
   1. Best Case Complexity.
3. Theta Notation
   1. Average Case

**Time**
1. Constant Time -> O(1)
2. Linear Time -> O(n)
3. Logarithmic Time -> O(logn)
4. Quadractic Time -> O(n^2)
5. Cubic Time -> O(n^3)