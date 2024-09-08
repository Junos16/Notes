# Algorithm Correctness

# Comparing Algorithms
- To solve a problem often there are multiple candidate algorithms that we could chose from. 
- To choose the best algorithm for a problem we need ways to quantify how well an algorithm performs
- Based on these metrics we might discard some candidate solutions for certain or all scenarios
	- ***Example:*** Insertion sort might be preferred over faster algorithms like merge sort and quicksort when N is guaranteed to be small due to its small constants being significant and better than other $\Theta(nlogn)$ algorithms
- The most common metrics we use to analyze algorithms include the run-time complexity and the memory complexity of the algorithm
	- Almost every algorithm aims to be fast and use the least amount of memory resources in the computer
- Depending on the context and the domain specific constraints we may wish to analyze certain other quantities as well
	- ***Example:*** Real world constraints on the cost of performing certain operations that aren't relevant to the execution of the algorithm. In the case of the Hiring Problem we want to hire the best possible candidate out of the applicants. Simultaneously we want to minimize the cost of hiring the best candidate as well.
## Asymptotic Analysis
- The metrics we are concerned with are functions of the input of the algorithm
	- ***Example:*** The run-time complexity of the algorithm depends on the number of inputs given to the algorithm. If we give a sorting algorithm 5 elements to sort vs 5 million elements to sort, naturally it would take more time to sort 5 elements
- Thus, to compare two algorithms using these metrics we would have to find a way to compare two different functions
	- ***Example:*** If we have two algorithms with the time complexity $T_{1}(n)=n$ and $T_{2}(n)=n^{2}$ then we can conclude that if they take 1 or more inputs the second algorithm is always faster since $\forall n\geq 1 \space n^{2}>=n \implies \forall n\geq 1 \space T_{2}(n) \geq T_{1}(n)$ 
- In most scenarios we won't have such a neat runtime for all algorithms. But given what we know about the input the algorithm is expected to receive, we can make approximations
- Most algorithms are expected to deal with very large inputs
	- ***Example:*** 
## Time Complexity
- When a computer program is being executed, then it is executing each instruction one at a time in sequence
- The time taken to 
### RAM Model
- 
## Memory Complexity
## Probabilistic Analysis
- While analyzing algorithms we might be interested in it's average case behavior more than the worst case behaviour
	- ***Example:*** Despite knowing that the worst case run-time complexity of Quicksort is $\Theta(n^{2})$ we often still prefer it over Mergesort (which has a worst case run-time complexity of $\Theta(nlogn$)). This is due to the fact that we know on average Quicksort has a run-time complexity of $\Theta(nlogn)$, the same as MergeSort but sorts the array in-place unlike MergeSort and has smaller coefficients for base cases
- To analyze the worst case behaviour of an algorithm we have to consider the very specific configuration that makes the algorithm behave the worst
	- ***Example:*** When trying to analyze the worst case run-time complexity of a sorting algorithm most often we know that the worst run-time occurs when the the array is sorted in reverse. Making this assumption about the nature of the input array helps us make the argument for what the worst case run-time complexity is
- But in the case of average case analysis we cannot make such an assumption, instead the analysis is more probabilistic in nature
- We cannot perform this analysis if we don't have some knowledge regarding the distribution of the input
	- ***Example:*** When finding the cost of hiring the best employee in the Hiring Problem we assume that permutation of the incoming applicants is uniformly random. So each $n!$ permutations of the input array are equally as likely 
- A way to deal with scenarios in which we don't know about the distribution of the input, but knowing something about the distribution of the input let's design good algorithms is to artificially impose a distribution on the input
	- An algorithm 
# Amortized Analysis