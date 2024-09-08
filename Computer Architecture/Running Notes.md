# Introduction
Why I might want to understand Computer Architecture:
- Being able to write good code in a world where optimizing for memory usage is irrelevant beyond the scope of embedded systems
- Being able to write programs that make use of parallelism and memory heirarchy
- Being able to write programs with energy efficiency in mind (especially in domains such as PMD and cloud)

What do i need to understand Computer Architecture:
- Understanding how high-level programs are converted to machine code
- Understanding how software interfaces with hardware
- Understanding how well a program performs
	- How does the original program, the compilation of program into machine code and the underlying hardware influence the performance
	- How could a programmer improve performance keeping all 3 aspects in mind (original program, compilation, hardware)
- Understanding hardware techniques to improve the performance of the program
- Understanding hardware techniques to improve energy efficiency
- Understanding the motivations for parallel processing and comparison of sequential and parallel processing

What factors impact the performance of a program
- The algorithm used to implement the program
	- Improve the run-time complexity of the algorithm
	- Improve memory complexity of the algorithm
	- Optimize for other costs/constraints
- The number of instructions needed to be executed (given by the compiler)
	- Reduce redundancy in the compiled instructions
	- Use best choice of instructions when there are multiple options
- How fast each of the instruction is executed
	- Improving processor performance to execute the same sequence of instructions faster
	- Improving how memory is allocated to make the same sequence of instructions use the faster memory hierarchies more often
- How fast I/O operations can be performed

Most important design ideas in computer architecture
1. Use abstractions to simplify design
2. Make the common case faster
3. improve performance via parallelism
4. Improve performance via pipelining
5. Improve performance via predicting
6. Use a hierarchy of memory
7. Improve dependability via redundancy

Abstraction in software
- A user might want to use a computer for a specialized task such as video editing or managing finances
	- In order to interact with the computer they would have to write instructions so that the computer understands what they want to do
	- This would make the process of video editing or managing finances extremely time consuming and complex
	- The user would have to think like a computer, in terms of low level management of memory, loops, binary arithmetic that isn't relevant to the task at hand
	- Abstracting out this process makes life simpler for the end user
- Application software > system software > hardware

Abstraction in hardware

# Instructions
Most modern computers are built based on the von-neumann architecture and thus largely perform the same fundamental operations
- There isn't much variation in most instruction sets across different devices due to this fact

Stored Program Concept: A computer can only recognize input in the form of high and low signals (represented using binary numbers) and use that to update the state in its memory (also stored as binary numbers)
- Thus we need to represent instruction the same way that we would represent data - as binary numbers

Design Principles:
1. Simplicity favors regularity
	- Example: while defining instructions like addition and subtraction, we only need a minimum of 3 operands: one that stores the result and the two operands that are to be added. despite allowing for more operands at the same time in more complex high level programming language, for a computer instruction set it is favored to just have the minimum requirements met as hardware for variable number of operands would be extremely complex
2. Smaller is faster

Variables/operands: 
- For most operations, the operands are limited to 32 registers on the hardware that are placed close to the processor
	- 