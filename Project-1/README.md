1. Which program is fastest? Is it always the fastest?  
    A.
     | filename  | # of blocks | time (sec) |
     | ------------- | ------------- | ------------- |
     | alloca.cpp | 1000000 | 0.154 |
     | alloca.cpp | 10000000 | 1.397 |
     | alloca.cpp | 100000000 | 13.694 |
     | list.cpp | 1000000 | 0.222 |
     | list.cpp | 10000000 | 2.073 |
     | list.cpp | 100000000 | 20.669 |
     | malloc.cpp | 1000000 | 0.169 |
     | malloc.cpp | 10000000 | 1.556 |
     | malloc.cpp | 100000000 | 15.326 |
     | new.cpp | 1000000 | 0.217 |
     | new.cpp | 10000000 | 2.039 |
     | new.cpp | 100000000 | 20.158 |

3. Which program is slowest? Is it always the slowest?
4. Was there a trend in program execution time based on the size of data in each Node? If so, what, and why?
5. Was there a trend in program execution time based on the length of the block chain?
6. Consider heap breaks, what's noticeable? Does increasing the stack size affect the heap? Speculate on any similarities and differences in programs?
7. Considering either the malloc.cpp or alloca.cpp versions of the program, generate a diagram showing two Nodes. Include in the diagram
   * the relationship of the head, tail, and Node next pointers.
   * show the size (in bytes) and structure of a Node that allocated six bytes of data
   * include the bytes pointer, and indicate using an arrow which byte in the allocated memory it points to.
8. There's an overhead to allocating memory, initializing it, and eventually processing (in our case, hashing it). For each program, were any of these tasks the same? Which one(s) were different?
9. As the size of data in a Node increases, does the significance of allocating the node increase or decrease?
