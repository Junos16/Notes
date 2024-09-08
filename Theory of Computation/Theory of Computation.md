- Given a problem, we would ideally like to have an algorithm to find the solution to that problem
	- Anyone could use the algorithm to solve the problem without having any understanding or expertise
	- There would be no room for ambiguity, guesswork, or human error
	- The solution would be reproducible and could essentially be automated 
- But we cannot take the fact that there exists an algorithm to solve a problem for granted
	- We might still be able to solve problems without an algorithmic solution but that solution might not be reproducible or automated
- We would thus have to demonstrate that there necessarily exists an algorithm that solves the given problem
	- For complex enough problems demonstrating the existence (or the lack of existence) of an algorithmic solution is much easier than finding an algorithmic solution
	- If we know about the lack of existence of an algorithmic solution then we could try to find heuristic solutions to the problem instead
- To be able to prove the existence of an algorithm for a problem we must first define the notions of algorithm and problem
	- In the context of Theory of Computation we use the notion of a ***Language*** to model problems
	- We model the intuitive notion of an algorithm or an ***Effective Method*** using a ***Model of Computation***
# Problems
- To model a computational problem, we use the notion of ***Language***
	- Every problem could be modeled as a language and its specific instances as a string in that particular language
	- ***Example:*** 
## Definitions
- For the purposes of Theory of Computation, our primitive is the notion of a symbol. Using this we will define alphabets, strings and languages
- ***Alphabet:*** An alphabet $\sum$ is a non-empty finite set of symbols
- **String:** A string is an ordered n-tuple $(a_{1}, a_{2},...,a_{n})$ such that $\forall k\in[1,n] a_{k}\in\sum$
	- ***Empty String:*** 
	- **Length of a String:**
	- ***Concatenation of two strings:***
- ***Powers of an Alphabet:***
- ***Language:***

# Algorithms
- To define the notion of an algorithm



- An effective method is a procedure for solving a problem 
- A method may be effective with respect to a class of problems but not be effective with another
- A method is considered effective for a class of problems if and only if:
	1. If consists of a finite number of exact, finite instructions
	2. When it is applied to a problem from its class:
		1. It always terminates after a finite number of steps
	    2. It always produces a correct answer
	3. In principle, it can be done by a human without any aids except writing materials
	4. Its instructions need only to be followed rigorously to succeed. In other words, it requires no ingenuity to succeed
## Model of Computation

# Complexity Theory
- Complexity of an algorithm is the algorithms run-time complexity (best, average or worst case)
- Complexity of a problem is the lower bound of any algorithm that can solve the problem
	- ***Example:*** The lower bound of sorting using comparisons is $O(nlgn)$
- 