## Binary and Decimal Number System.


### Decimal to Binary.
- Check handwritten notes for the first approach.
- 2nd Approach is as follows :
  - Any number when & with 1 gives 1 if the number is odd and it gives 0 if the number is even.
  - This is because 1 is 0000.....000001, so all the previous bits except the last bit after AND is going to be 0. The last bit, if it is 1 will give 1 in the output and the last bit if it is 0 will give 0 in the output.
  - If the last bit is 1, the number is odd because 2^0 * 1 = 1 which will be added to the even powers of the number.
  - So the approach is to find the last bit n by doing '&' with 1, then right shifting the number until n is 0.
  - **IMPORTANT : Whenever we do binary operations on decimal numbers such as '&' or '>>' or '<<', the operation performed on them is in binary i.e. in bits but we still get the final output in decimal.**