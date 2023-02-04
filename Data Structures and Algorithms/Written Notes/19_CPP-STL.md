  
# CPP-STL
  
---
References
1. [Love Babbar Whimsical](https://whimsical.com/c-stl-XVxuHHof5GTWA4NXZhXQhx)
2. [Backup Whimsical](https://whimsical.com/c-stl-NJwztDUeLn7LWuCRRySR1G)
3. STL Data Structures Iterators: [[CPlusPlusNotesForProfessionals.pdf#page=35]]
---

### Array
- The implementation of the STL array is same as that of the basic array.
- That is, the STL array is also static which is the reason that it is not mostly used.
- Refer [[CPlusPlusNotesForProfessionals.pdf#page=281]]
- Array Operations: 
   1. `arr.size()`- Helps to find the size of the array. (Complexity : O(1))
   2. `arr.at(index)` - Helps to find the value present in the array at the given index. (Complexity : O(1)) 
   3. `arr.empty()` - Helps to find if the array is empty or not. (Complexity : O(1))
   4. `arr.front()` - Returns the first element of the STL array. (Complexity : O(1))
   5. `arr.back()` - Returns the last element of the STL array. (Complexity : O(1))
---

### Vector
- Refer [[CPlusPlusNotesForProfessionals.pdf#page=285]]
- Vector is simply a dynamic array.
- Just like array, elements in vector are also stored in contiguous memory locations.
- The difference is that when you add an element in a vector which is full, the vector will double its size.
- The way it does this is that, it will create another vector which is double the size of the current vector and then it will copy all the elements of the current vector to the another vector and will dump the current vector. Can also decrease the size using to fit.
- Initialising a vector.
   - We can create a vector without specifying the size.
   - The size of the vector during its creation in such case is 0.
   - If we know the size of the vector, we can specify the size of the array as shown in the code and can initialise all the elements of the vector with a given value.
   - The size of the vector denotes how many elements are present in the vector, and the capacity denotes for how many elements, the vector contains space.
   - In order to create a vector with the values of another vector, we can just specify the vector to be copied in brackets when initialising new array. For example `vector<int> b(a)`
   - Here, the elements of the vector a will be copied into b.
   - We can also initialise it as `vector<int> a(5,1)`, here the size of the vector a is 5, and all the elements are initialised with 1.
- Vector Operations:
   1. `vector.capacity()` - Indicates the vector capacity, that is, for how many elements the vector contains space.
   2. `vector.size()` - Indicates the vector size, that is, how many elements are actually present in the vector.
   3. `vector.push_back(ele)` - Is used to push the element(ele) into the vector. 
   4. `vector.at(index)` - Helps to find the value present in the vector at the given index.
   5. `vector.front()` - Returns the first element of the STL vector.
   6. `vector.back()` - Returns the last element of the STL vector.
   7. `vector.push_back(ele)` enters the element to the last index in the vector 
   8. `vector.pop_back()` - removes the element present in the last index of the vector.
   9. `vector.clear()` - It is used to clear the vector, that is, remove all the elements present in the vector. One thing to note here is that when the vector is cleared, only the size becomes 0, but the capacity remains the same as that of before clearing.
   10. `vector.begin()`- If starting iterator of the vector is required, we can use the begin.
   11. `vector.end()`- If ending iterator of the vector is required, we can use the end.
- The iterator methods are used to point to the first and the last element.

---

### Deque
- Also known as Doubly ended queue.
- Can perform push-pop, that is insertion-deletion at both the ends, that is at starting as well ending of the deque.
- Unlike array and vector, values are not stored in contagious memory locations in deque.
- Here, there are multiple fixed static arrays and tracking is done that data is present in which array.
- Deque is also dynamic, random access is also possible (using at).
- Deque operations: 
   1. `deque.begin()` -  If starting iterator of the deque is required, we can use the begin.
   2. `deque.end()`- If ending iterator of the deque is required, we can use the end.
   3. `deque.push_back()` - Is used to push the element at the back of the deque.
   4. `deque.push_front()` - Is used to push the element at the front of the deque.
   5. `deque.pop_back()` - Is used to pop the element at the back of the deque.
   6. `deque.pop_front()` - Is used to pop the element at the front of the deque.
   7. `deque.at(index)`
   8. `deque.front()`
   9. `deque.back()`
   10. `deque.empty()`
   11. `deque.size()`
   12. `deque.erase(iterator1, iterator2)` - Is used to erase the specific elements from the deque. In case of just specifying one iterator, it will delete one element, and in case of providing two iterators, it will delete range of elements where the element at the first iterator is included and the the element at (iterator2-1)th index is included. Refer [Deque Clear and erase](https://www.geeksforgeeks.org/dequeclear-dequeerase-c-stl/)
7.  After emptying, in deque as well, the size will become 0, however, the capacity will remain the same.
---

### List
- The list STL is created with the help of doubly linked list.
- Refer [[CPlusPlusNotesForProfessionals.pdf#page=]]
- In doubly linked list, there are two pointers, one for the front and other for the back.
- Direct access of the elements with the help of square brackets or with the help of at function as in arrays, vectors, deque is not possible in list.
- In list case, we need to travel to the fourth element, in case we want the fourth element.
- List Operations
   1. `list.begin()`. - O(1)
   2. `list.end()`. - O(1) 
   3. `list.empty()`. - O(1)
   4. `list.front()`. - O(1)
   5. `list.back()`. - O(1)
   6. `list.push_back()`. - O(1)
   7. `list.pop_back()`. - O(1)
   8. `list.push_front()` - O(1)
   9. `list.pop_front()` - O(1)
   10. `list.erase(l.begin() or l.end())`. - O(n)
   11. `list.size()` - O(1)
---

### Stack
- Last In, First Out.
- In stack, there are two main operations, one being push and the other being pop.
- The element which is entered at the last is the element which first comes out when the pop operation is applied on the stack.
- Stack Operations.
   1. `stack.push(element)`.
   2. `stack.pop()`.
   3. `stack.size()`.
   4. `stack.empty()`.
   5. `stack.top()` - Returns the top element that is the element which is entered latest into the stack.
---

### Queue
- First in, First out.
- It can just be considered a normal queue as in case of theatre ticket queue, bouquet queue or just any other queue.
- The element which is entered at the first is the element which first comes out when the pop operation is applied on the queue.
- Queue operations.
   1. `queue.push(element)`.
   2. `queue.pop()`
   3. `queue.size()`
   4. `queue.empty()`
   5. `queue.front()` - Returns the first element of the queue.
   6. `queue.back()` - Returns the last element of the queue.
- All the operations have a complexity of O(1). 
---

### Priority Queue
- In priority queue, the first element is always the greatest just as in case of max heap.
- The default priority queue is max heap.
- In case of max-heap and priority queue, whenever you fetch the element, the element will be of largest value.
- In case of min-heap, whenever you fetch the element, the element will be of minimum value.
- When you initialise priority queue as `priority_queue<int> maxi`, it is based on max heap, which means when we fetch the element, the element will be greatest from the elements stored in the priority_queue.
- In order to create min heap, we can declare priority queue as `priority_queue<int, vector<int>, greater<int>> mini`.
- Refer the code, when printing the top element of the priority queue and popping the element of the priority queue, we first store the size of the priority queue in a variable rather than doing it in the for loop as `i<maxi.size()`, this is because at each iteration the size of the 'maxi' will keep on changing as in each iteration, we are popping the element out of the queue.
8. Priority Queue operations
   1. `pq.push(ele)`
   2. `pq.pop()`
   3. `pq.top()`
   4. `pq.size()`
   5. `pq.empty()`

### Set
- Refer [[CPlusPlusNotesForProfessionals.pdf#page=318]]
- Refer [Set Iterators](https://www.geeksforgeeks.org/setbegin-setend-c-stl/)
- The important property of a set is that it just has all the unique elements stored inside it.
- For example, if you store a single element, let's say 5, for 5 times, then too 5 will be stored just for a single time.
- It stores all the elements just for a single time and its implementation in the backend is done using BST.
- Once the element is inserted, the element cannot be modified, either enter the element or delete the element, but you cannot modify the element.
- Elements are returned in sorted order.
- The difference between unordered set and set is that set is little slow than unordered set and in unordered set elements are returned in unsorted order.
- Set operations
   1. `set.insert(ele)` - Is used to insert an element into a set. Complexity - (Ologn)
   2. `set.erase(iterator)` - It is used to erase or delete a particular element in the set with the help of an iterator.
   3. `set.begin()` - Iterator pointing to 0.
   4. `set.count(ele)` - Lets us know whether the element is present in the set or not. The output may be 0 or 1.
   5. `set.find(ele)` -  After finding the element, it returns us the iterator/index of the element.

### Map
- Refer [[CPlusPlusNotesForProfessionals.pdf#page=287]]
- Map is a data structure in which the data is stored in the form of key-value pair.
- Each and every key is unique and a single key points to only one value. A key points to just a single value and it then cannot point to any other value.
- There can be 2 keys pointing to same value, however there cannot be 2 values pointing to one key.
- The output of the map is in sorted order and in case of unordered map, it is not in sorted order.
- The complexity for insert, erase, find, count, etc. in case of map is O(logn).
- The ordered map is implemented with the help of red-black tree or balanced tree and the complexity for search here is O(logn).
- In case of unordered map, the implementation is done using hash table and the complexity for search in that case is O(1).
- Map Operations
	1. `map.insert({key,value})` - It is used to insert a key-value pair in a map.
	2. `map.erase(key)` - In the case of map, we need to specify the key to erase the key-value pair instead of the iterator  as seen in the other data structures.
	3. `map.begin()` - Already known.
	4. `map.end()` - In both, the begin and end, we need to specify the first or second in order to print the key or value respectively.
	5. `map.find(key)` - Returns the iterator of the key.

### Algorithms
- We can find a particular element with the help of **binary search**, that is O(logn) complexity with the help of STL binary search.
- The syntax for the same is: 
  ```CPP
  binarySearch(vector.begin(),vector.end(), ele);
  ```
- Here, vector.begin() and vector.end() are the starting and ending iterators respectively and ele is the element which is to be found in the vector.
- Finding upper bound and lower bound, refer code and [GeeksforGeeks](https://www.geeksforgeeks.org/upper_bound-and-lower_bound-for-vector-in-cpp-stl/)
- Max and min of two elements.
- Swapping of two elements.
- Rotation of a vector (We need to specify the start iterator, how many elements we want to rotate and the end iterator).
- Sorting of a vector. It is based on intro sort which is the combination of three algorithms which are quick sort, heap sort and insertion sort. All these three algorithms together make up to intro sort which is behind the scenes of the sorting.