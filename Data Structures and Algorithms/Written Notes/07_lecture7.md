## Leetcode Problem Solving.

### Reverse Integer Problem
- In the reverse integer problem, for the normal condition we should just do the normal reverse problem with the formula 
rev = rev*10 + rem.
- The key thing here is the other condition which suggests that if the reversing of integer causes the integer to go out of the int limit while applying the above formula, we must return 0.
- For solving this, we must apply an additional if condition where we check if rev > (INT_MAX/10) || rev<(INT_MIN/10). In either of the cases, we must return 0.
- Personal doubt : The doubt I had was that the rev > INT_MAX/10 + rem. Because, we are also adding the remainder. Here though, if the number is greater than INT_MAX/10, it is obvious that the number is also greater than INT_MAX/10 + rem.
- Also, the reverse will overflow in the point 1 formula during the rev*10 itself, if we do it INT_MAX/10 + rem. This is because, we are returning 0 only in this case, any number lower than this won't return 0 and INT_MAX/10 would still be accepted which will cause the integer to overflow.
- INT_MIN is done because negative numbers are also given which returns answer in negative.


### Is Power of Two
- In the first solution, in order to check if the number is a power of two or not, we need to compare number with all powers of 2 ranging from 0 to 30. (30 because the positive range of number ranges upto 2^31-1, and therefore 2^31 in itself is not included.)
- In order to optimize it, the other solution is that we can use existing answer, that is initialize answer with 1 and then keep on multiplying it by 2 for each iteration. 1x2 = 2, 2x2 = 4, 4x2 = 8, 8x2 = 16 which is exactly what a power does. But in this case, we are just reusing the value of answer.
- The third solution is with the help of bits. We need to find out if the given number is a power of 2, we know that the number will have exactly one set bit if it is a power of 2. For e.g. 32 - 100000. Therefore, we can maintain a count of the set bit the input number has. In order to check the count, we can simply '&' the number with 1. If it comes out to be 1, we add 1 to the count or else we don't add one to the count. In both the cases, we will right shift the number. If the count of the set bits comes out to be exactly 1, we can conclude that the number is a power of two.