1. Swap Alternates
   1. In the first approach, we maintain two variables throughout the loop, one is the count for which the loop runs which is `count<size/2` as we are comparing 2 elements withe each other and in case of odd number of elements, we can safely ignore the last element in the array. The second variable is for pointing the index so that we can compare two elements with each other.
   2. In the second approach, we are checking if the (i+1)th element is less than n. The i here is similar to the pointer in the first approach, however instead of having another variable as count, we are just checking if the value (i+1)th element is less than n. This is because in the edge case in odd number, the ith element will be less than the size however, the (i+1)th element will be equal to the length of the array.


2. Find Unique
   1. In the **first approach**, we first go for each element and compare each element to all the other elements except itself. If it turns out to be equal to itself, we skip that particular iteration using continue and then compare the number with all the other numbers. 
   2. If the number turns to be equal to some number, we set the flag as 1 and break out of the loop to check the other number.
   3. If the number is not equal to any other number, the flag will remain 0 as initialized and then it can be considered as unique number which we will return to the main function.
   4. As we know, returning a value marks the end of the function, so we won't compare further values as well.
   5. In the **second approach**, we initialize unique as 0 and then XOR, with all the elements in the array.
   6. We know that 0^a = a and a^a = 0. Therefore, all the duplicate elements when XOR'd will become 0 and the final output will be the unique element.

3. Intersection of Two Arrays
   1. 1st solution
      1. For each element in arr1, check if there is same value in arr2.
      2. If yes , print the value and then update the value in arr2 to a value like INT_MIN so that the same value is not matched again and then break so that same value is not matched in case of duplicate in 2nd array.
   2. 2nd solution (Optimised)
      1. Here, we are having three conditions, that is if the element in the first array is less than the element in the second array, we will increase the count of the index in the first array as there will be no match in the 2nd array due to the increasing order of elements.
      2. If both the elements are equal, then we will increase both i and j.
      3. If the element in j is less than the element in i than, we will increase j as again no element will be matched in i due to the increasing order just like the first case.
      4. The loop will go on until i and j are equal to the length of the array.
<br>

4. Pair Sum: <br>
https://www.codingninjas.com/codestudio/problems/pair-sum_697295
   1. We will be making use of two loops for this problem namely i and j.
   2. i will be starting from 0 and j will be starting from i+1, i.e in each iteration of i, we will be comparing with i,  all the elements ahead of i(i.e j) and check if it equals to the sum.
   3. We will first be creating an **ans** variable which is vector of vector int as we need to return multiple pairs.
   4. Secondly, we will be having **temp** which is a vector int for each of the individual pairs.
   5. Based on the condition, in each pair, we need to ensure that the first number in the pair is smaller than the second number so we will be pushing the smaller number in the temp first and then the larger number.
      ```
      The condition: Each pair should be sorted i.e the first value should be less than or equals to the second value.
      ```
   6. Then we will push the temp to the ans.
   7. After pushing all the pairs to the ans, we will sort the ans again based on the condition and thus we will get the output.
      ``` 
      The condition : Return the list of pairs sorted in non-decreasing order of their first value. In case if two pairs have the same first value, the pair with a smaller second value should come first.
      ```
<br>

5. Find the duplicate element in an Array.
https://www.codingninjas.com/codestudio/problems/find-duplicate-in-array_1112602
   1.  Explained the XOR method in notebook.


6. Triplets with given sum: <br>
   1. We will have the same approach as that of the pair sum.
   2. Here first we will take i as 0, j as i+1 and l as j+1.
   3. Then we would check if the value of all these three are equal and if they are equal, then we will first sort it.
   4. After sorting we would temporarily store it in a set so as that no values are repeated.
   5. We need the ans in the vector variable ans, so outside of for loop, we would iterate in each value of s using the auto x which iterates through each value of s and then we would push each x into the ans.
   6. And then we would return the ans.
   7. Also, the reason auto is used here is that it automatically assigns data type to x. That is during compile time, when the compiler reaches x, it will detect the type of x from initialization and accordingly give it a data type in this case, vector.
   8. Read more about it here: https://whimsical.com/c-stl-XVxuHHof5GTWA4NXZhXQhx
