# [Heap]( http://en.wikipedia.org/wiki/Heap_\(data_structure\) ) Implementation in C++

This is an implementation of a **binary heap**.   
Heaps maintain an implicit binary tree structure in an array.


##Operations
*n* = number of items in the heap

- **Insert** - *O(log n)*: add a new item to the heap
- **Extract min** - *O(log n)*: remove an item with minimum value    
- **Delete** - *O(log n)*: remove an item from the heap
- **bubbleUp/bubbleDown** - *O(log n)*: rearrage heap to maintain its property
- **Heapsort** - *O(n log n)*: calls extract-min *n* items to sort the heap
- **Make heap** - *O(n)*: given an unsorted array, each element for *n* elements has to be added into the internal queue and bubbleDown *O(log n)*. Not all heapify operations are *O(log n)*, this is why you are getting [O(n)](http://www.cs.umd.edu/~meesh/351/mount/lectures/lect14-heapsort-analysis-part.pdf).  


## Random Trivia
max-heap vs sorted array:   

1. Find the maximum element quickly:    
O(1) for both. Root of max-heap and last element in array.    
2. Delete an element quickly:   
O(log n) for max-heap. O(n) for array without the element index, otherwise, O(1).   
3. Form the structure quickly:  
O(n) to build a heap, O(n log n) to sort an array.      
4. Find the minimum element quickly:  
O(log n) to find the min element. O(1) for the array as the first element. 
