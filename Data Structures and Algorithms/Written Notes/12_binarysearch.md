# Binary Search

1. **Binary search only applies in monotonic functions.**
2. Monotonic functions are those functions which are either in increasing order or either in decreasing order.
3. If start = 2^31-1 and end = 2^31-1 which is the highest limit of the integer, then in line no.8 when we do (start+end)/2, in the operation of '(start+end)', our integer can go out of bound and may give an error.
4. So we can modify this formula as s + ((e-s)/2) which will result in (2s+e-s)/2 and in return it gives (s+e)/2 which is the correct original formula.
5. Advantage of Binary Search
   1. Suppose if there's an array of size 1000.
   2. In the worst case, in linear case there will be 1000 comparisons.
   3. In binary search, first the array is of size 1000, the, 500-->250->125->62->31->15->7->3->1->0, that is just 10 comparisons.
   4. In linear search, the complexity is O(n) whereas in binary search, the complexity is O(logn).
   5. https://www.geeksforgeeks.org/complexity-analysis-of-binary-search/