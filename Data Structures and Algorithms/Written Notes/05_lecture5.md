  ### NOT (~) Operator
- When taking NOT, we first not the number using '~'. For example ~2. 
- This will invert all the bits of 2. That is 2 = 000000......00010.
- Inversion = 1111111.......1111101.
- The first bit will represent that it is a negative number.
- Then take two's complement of other bits = 0000000.....0000011.
- Which is equal to negative three.
- **1 is known as set bit.**

### Left Shift and Right Shift
- When **left shifting** a number, think that the output will get multiplied by the original number.
- This happens in majority of the cases (usually small numbers) and it does not happen in every case.
- The reason it does not happen in every case is that suppose if the second bit is one and then we left shift for e.g 010000000......00000.
- Then after left shifting this binary number we would get 10000000.....000 which shows the MSB as 1 and represents negative number.
- When **right shifting**, the output is divided by 2 of the original number.
- In case of positive numbers, padding is always done with 0 in right shift and left shift. 
- However, in case of negative numbers, padding is compiler dependent. 
- We don't know what the compiler might do, it is dependent on the compile.
- 
### Post increment and pre-increment
- Explained in Lecture 5 PDF Notes.


### For loop
- Basic for loop explained in the PDF Notes.
- Initialisation, condition and updation are not necessary and can just have semicolon.
- for( ; ; ){
    ....
    ....
}
- Example:
int i = 1;
for( ; ; ){
    if(i<=n){
        cout << i << " ";
    }
    else{
        break;
    }
    i++;
}
- Using multiple inits, conditionals and updations.
for(int a = 0, b = 1, c = 2; a>=0 && b>=1 && c>=2 ; a--,b--, c--){
    cout << a << " " << b << endl;
}

### Variables and scopes
- Explained in PDF Notes.


### Leetcode Questions.
1. Subtract the product and sum of digits of an integer - https://leetcode.com/problems/subtract-the-product-and-sum-of-digits-of-an-integer/
   - Here we will first take out the digit by dividing it by 10 and taking the remainder. For example, if the number is 123, after dividing it by 10, we will have the remainder 3. We will multiply it with the product which is initialized by 1 and add it to the sum which is initialized by 0.
   - Next we will, divide the number by 10 so as to pull out other digit by again taking out the remainder from 10.
   - That is 123/10 = 12. 12 % 10 = 2.
   - 12/10 = 1. 1 % 10 = 1.
2. Number of '1' Bits - https://leetcode.com/problems/number-of-1-bits/
    - The number of '1' Bits an integer has is also known as hamming weight.
    - Check DSA Book Page 12.
3. Reverse Integer
   - One important condition given in the description is that if the number is greater than the 32-bit integer range, then return 0. 
   - Therefore, we are having an if condition where we check if the rev of the x, is greater than the signed 32 bit integer range. 
   - We are checking, if the number is greater than INT_MAX (integer range)/10. 
   - The reason we are dividing by 10 is that as soon as we multiply it by 10, when reversing it, it would cause the rev value to overflow and therefore we are checking it in advance.