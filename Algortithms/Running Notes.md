# Running Notes algorithm analysis

Real world problems - generally complex, multivariate, amorphous, not-well defined
	require trial and error and experience

Some problems instead are well-defined(have clear requirements, conditions and constraints
Solutions for these problems can be definitely ruled as correct or incorrect
	can be analysed and compared quantitatively
	not necessarily easy to find but can be formally analyzed

These types of problems are thus of special interest to us.
	Non-well defined problems can often be reduced to well-defined problems to have some way to approach them

The solutions (algorithms) to such problems involve a finite number of steps that necessarily provide the required solution
We use heuristic solutions to solve non-well defined problems
	domains in which there is no well-defined condition for correctness and/or optimality of solution
	Heuristic solutions use some

Note: even non-deterministic problems can be well-defined and analysed using prob

-- read about heuristic and approximate algorithms
	are all heuristic solutions used to solve non-well defined problems (such as recommender systems)
		some seem to be used to speed up   

## How to prove that an algorithm is correct?

Notion of algorithm correctness:
	Functional Correctness: If for all input in the domain of the algorithm a satisfiable output is returned but the algorithm
	Partial Correctness: For some input in the domain, if an output is returned then the output is correct
	Total Correctness: For all input in the domain, an output is returned and the output is correct

	
## Time Complexity Analysis
	Since we have a well-defined finite solution to a well-defined problem,
	aside from checking for the correctness of the particular solution we can also
	compare the quality of two alternative solutions

	potential metrics to be used to compare the two solutions:
		time taken to execute
		amount of memory required to execute
		baandwidth etc
	
	depending on the domain different metrics for comparing algorithms can be considerd
		for numerical methods we might consider numerical accuracy
		in the domain of distributed systems we consider communication complexity
		parallelizability is considered in parallel processing domain
	
	generally the most common parameters to consider include time and memory complexity of an algorithm
	

	to measure the time complexity of an algorithm we need to have an abstract way to measure the time required to execute an algorithm
		we must ignore real world physical limitations in the processors being used 
		we must also ignore nuances of the implementation of instruction in rams (concurrency, variation in cost of execution of different intructions)

	assume that standard instructions that we would realistically use in any ram would have same constant cost
		for example ignore nuances in the time complexity of an exponentiation instruction that can change based on the base
		ignore nuances of data types being used and their precision (though this is important in real world implementations of programs)
		
## Divide and Conquer

	