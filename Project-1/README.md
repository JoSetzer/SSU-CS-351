| filename  | # of blocks | 3/100 time (sec) | 100/1000 time (sec) |
| --- | --- | --- | --- |
| alloca.cpp | 1000000 | 0.154 | 1.180 |
| alloca.cpp | 10000000 | 1.397 | 11.643 |
| alloca.cpp | 100000000 | 13.694 | 114.979 |
| list.cpp | 1000000 | 0.222 | 1.234 |
| list.cpp | 10000000 | 2.073 | 12.270 |
| list.cpp | 100000000 | 20.669 | 160.579 |
| malloc.cpp | 1000000 | 0.169 | 1.160 |
| malloc.cpp | 10000000 | 1.556 | 11.450 |
| malloc.cpp | 100000000 | 15.326 | 126.195 |
| new.cpp | 1000000 | 0.217 | 1.230 |
| new.cpp | 10000000 | 2.039 | 12.102 |
| new.cpp | 100000000 | 20.158 | 120.970 |


1. Which program is fastest? Is it always the fastest?  
    A. According to the times recorded above with the default makefile properties, the fastest process consistently was the program using the alloca function
2. Which program is slowest? Is it always the slowest?  
    A. The list and new programs were extremely close in execution time; however, the list was slightly slower consistently than the new.
3. Was there a trend in program execution time based on the size of data in each Node? If so, what, and why?  
    A. The table above was collected with MIN_BYTES = 100 & MAX_BYTES = 1000 data in the fourth column. Comparing the time to complete between the third and fourth columns, we can see that an increase in node size correlates with a direct increase in execution time.
4. Was there a trend in program execution time based on the length of the block chain?  
    A. Increasing the blockchain length increased the time to complete for each process exponentially.
6. Consider heap breaks, what's noticeable? Does increasing the stack size affect the heap? Speculate on any similarities and differences in programs?  
    A.
8. Considering either the malloc.cpp or alloca.cpp versions of the program, generate a diagram showing two Nodes. Include in the diagram
   * the relationship of the head, tail, and Node next pointers.
   * show the size (in bytes) and structure of a Node that allocated six bytes of data
   * include the bytes pointer, and indicate using an arrow which byte in the allocated memory it points to.
9. There's an overhead to allocating memory, initializing it, and eventually processing (in our case, hashing it). For each program, were any of these tasks the same? Which one(s) were different?
10. As the size of data in a Node increases, does the significance of allocating the node increase or decrease?
