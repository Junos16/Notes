Scenario:
    Trying to write a program in assembly to swap the contents of two blocks of memory
    Need 2 blocks of memory where i will be storing the contents to be swapped
    Need another block of memory to act as placeholder


Scenario:
    - Writing a program in C that has a main function
    - When program is compiled and ran, it needs memory to store values
    - At the start of the program it makes sense for the OS to allocate it some amount of memory
    - Say that the program has 2 16bit integers that it is storing then at the start of the program the OS only needs to provide it with 32 bits of memory to store values in
        - It can store it from the start address and store them contiguously
    - If we call a function from the main function we want to have a separate memory space for the variables inside the function (separation of scope) 
        - We can keep track of the starting memory address of the function's memory space and then store all variables contiguously inside it
        - When the function stops executing we can move the stack pointer back to the start of the functions memory space to free it. 


Stack:
- We need fast allocation and deallocation
    - For deallocation we want it to just be a pointer being moved to the position after which the memory is being written
    - For allocation we just want to write immediately to assigned memory
- For that we need to have the point after which memory is free at all times
    - 

Summary
- Compact data
    - Avoid external fragmentation
    - Increase cache hits
- Predictable behavior
    - Fast allocation
    - Easy to handle function calls and local data
    - Fast deallocation
- Large data causes overflow
- No dynamically sized data allowed
- Single Threaded


Current Understanding

- We want a processes accessible memory to be isolated (virtual memory)
- When a process is created after a program is executed OS gives it it's memory
- We want the memory allocation and deallocation to be fast and efficient
    - Memory not being allocated contiguously would lead to external fragmentation
        - To maintain contiguous memory storage programmers have to be prevented from resizing their variables after compile time
        - They cannot declare dynamically sized variables or variables with no specified size (like vectors)
        - Thus at compile time programmer must specify the size of the programs (procedure's) variables
    - Any form of lookup or adjustment of the existing memory would be very slow
        - To avoid adjusting existing memory, allocations must be performed after the allocated memory locations end
            - To avoid lookups we must maintain the address of the memory location where allocated memory ends
    - A stack like allocation/deallocation strategy models these requirements very well
        - A sequencial memory allocation approach works well to maintain contiguous storage
        - Maintaining a pointer to the end of the allocations means one directional allocation
        - Deallocation must also occur in a contiguous and predictable manner
            - The size of the allocated blocks of memory associated with each variable in the program must be known at compile time so that the process doesn't accidentally deallocate something other than what it was trying to deallocate
            - Deallocation is trivial as it just moves the stack pointer to the point where the deallocated chunks of memory starts
            - Stack based deallocation strategy is more tied to the control flow of function calls/thread spawning 
        - Any relatively simple linear data structure with restrictions on allocations would work well for this task 
            - Restricting memory allocations in a certain direction allows for contiguous allocations and fast allocations as well (can't have this with indexed direct allocations)
            - Stacks restrict allocations to the top modelling control flows where the oldest allocation is the most important and needs to persist the longest
                - Memory associated with parent functions must persist longer than the memory associated with a function call or a thread spawned
            - Queues restrict allocations to the ends, could be used as well
                - But queues model scenarios where the most recent allocation is what we want persisting the longest
            - ***QUESTION:*** Was stack based model the consequence of the way program control flow worked or was it the other way around?
- When we want to allocate memory in ways that this model allow for then we have to start making tradeoffs in terms of speed and memory efficiency
    - To have access to resizable variables we can't allocate them contiguously
    - To be able to have variables of unspecified sizes we would have to also sacrifice contiguous allocation
    - To still have relatively fast access to the memory we need to maintain ways to lookup chunks of memory separately requiring more memory usage
    - Lookup tables or pointers to memory chunks allow relatively more efficient memory allocation (preventing fragmentation) by tracking free memory and allocating discontiguously
    - Thus, we would need to have a completely separate chunk of memory associated with a process that has separate rules for allocation, access and deallocation
        - Memory might be allocated initially contiguously at the start, but if the variable's size is modified at runtime then some sort of a pointer/linked list/lookup table based approach is used to index the separate discontiguous chunks of memory
        - Allocation is much slower due to having to look up which parts of the chunk of memory are free and which are in use
            - Moreover any sort of pointer/lookup table structure needs to be updated after the allocation
        - Deallocation isn't as easy as just moving the stack pointer
            - Updates to the pointer/lookup table structure is again performed
- Something else that is relevant in memory allocation strategies is determining the owner of the memory
    - The OS utilizes virtual memory to maintain isolation of the memory space for programs
        - This provides abstraction that simplifies memory management for the programmer
        - The programmer has to only be concerned with the way memory is handled inside the program (treating as if the program has access to the whole device's memory)
        - They no longer have to worry about accidentaly writing to memory space dedicated to another process
        - It's also cheaper for large amounts of memory as we don't need to add more information per unit memory allocated to identify the process it is associated with 
            - This approach could work in very small cases, but when you need multiple bytes to identify the process id it becomes too expensive
            - Schemes like paging are used to identify the physical address of the memory location associated with a process without costing a lot of extra bits or requiring the programmer to keep track of the physical address
    - This isolation could be adapted to provide more convenient abstractions within the process itself
        - Instead of letting the programmer have to deal with a monolithic sequence of instructions performing a lot of complex tasks it is easier to break it down into smaller chunks and then orchestrate their executation by specifying the control flow (order of execution)
    - Just like with memory associated with different processes it might be convenient to let the programmer treat the memory associated with each of these chunks of instructions as it's separate program
        - When a procedure/function is called or a thread is spawned by the main process it could create a separate *stack* of memory specifically dedicated to it
        - The programmer treats this *stack* as all the memory available to the procedure/thread that is currently being ran by the parent process
        - When a process ends executing then the OS reclaims the memory allocated to the process. This idea extends to the procedure/function as well
        - When the function stops executing it's stack must be deallocted by the parent process
    - Unlike at the process level where schemes like paging are used, a function or a thread's stack could easily just be allocated to the process's stack
        - This is due to the control flow of function calls and threads spawned
        - When a new function is called or a thread is spawned we need to transfer control to the new function/thread
        - After they are done executing we switch back to the parent process
        - Thus the way we treat the memory associated with them is similar to how we treat memory allocated to the stack, the most recently allocated memory is least necessary to persist
    - For any process thus only a single stack is maintained
        - The function's/thread's variables are allocated to the stack with some sort of a delimiter
        - Each time a new thread is spawned or a function is called we push it's stack to the process stack
        - As usual we know the size of the variables local to the function or the thread ahead of time
        - If a function is due to return some value of some specified size then we reserve that amount of memory before the function's stack is pushed and when the function stack is popped we write the return value to that memory address
    - This approach creates the desired isolation for threads and function calls
    - But if we want more flexibility in terms of ownership of the memory i.e. letting more than one thread access a memory location or persisting the data allocated to a memory location inside a function after the function returns then we need to again make tradeoffs
        - ***QUESTION:*** Why don't we have a heap associated with each function/thread? we could always a global heap as well

- Outline of argumentation:
    - We want to provide a process with some amount of memory to work with isolated from other processes
    - We want memory allocation in provided memory to be fast and efficient (no wasted memory)
        - We provide each process with a fixed amount of memory that they must work with
            - Asking the OS for more memory is slow thus they must restrict themselves to this region of provided memory if they don't want optimal speed
        - Memory allocation is restricted to contiguous chunks to improve locality 
        - Sequential memory allocation with fixed variable sizes prevents fragmentation and makes allocation and deallocation very fast (only 1 instruction)
            - Maintaining a pointer to the location where allocated memory ends is enough to keep track of free and used memory as all the used memory is chunked together
            - Any allocation and deallocation just requires moving the pointer at tne end which is very fast and doesn't require the use of any sophisticated lookup tables or linked structures with more than 1 pointer
            - This restricts the programmer from extending the size of a variable and declaring variables with unspecified sizes
    - We want to handle memory allocations related change in control flow gracefully
        - Each function call/thread spawned requires it's own isolated memory with local variables
        - Maintaining these chunks of memory on the same chunk as the parent process is convenient 

- Processes need memory to allocate variables and work with them isolated away from the rest of the system
- Ideally we want the memory allocation and deallocation to be extremely fast and make efficient use of the given memory
    - Solution: 
        - Don't make the process ask the OS for memory after it has been allocated once as providing more memory is very expensive, assign an initial fixed amount of memory based on requirements and 


- Fast and efficient memory management
- Handling control flow
- Scoping
        - 
