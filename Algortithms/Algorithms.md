## Algorithms

##### What are Algorithms?

- Problems that arrise in the real world often require *trial and error*, *guesswork*, *intuition*, *human interpretation* and other subjective/non-concrete tools to arrive at a solution. This increases the chances of errors, inaccuracies and inefficiency.

- It would be preferrable if all problems only involved concrete descriptions and required objective step-by-step solutions. These problems are called *algorithmic problems* and the procedures required to solve them are called *algorithms*. 

- The benefit of such a scenario would be the elminitation of factors mentioned above (*trial and error*, *guesswork*, *intuition*, *human interpretation*, etc). This implies massive reduction in the chances of committing errors and allows for automation of the problem solving process.

- The first kind of problems are ***Heuristic Problems***, as opposed to the other kind ***Algorithmic Problems***. 

- Example: Loosing weight vs Allocating time to daily tasks based on fixed priorities. 

##### Algorihtmic Solutions in the Real World

- The best case scenario is that we have the exact algorithm needed to solve a problem already at hand. It is then only a matter of execution. A slightly more inconvinient scenario is when the problem differs from a previously known algorithm at a surface level, but can be abstracted to be effectively the same problem.

- In most cases we will not have a direct route to an algorithmic solution. It could be the case that we are not aware of pre-existing algorithms that could be used to solve the problem, or it might be that no such algorithm exists in the first place

-  Also we might not have a well-defined problem in the first place. In such a case one viable strategy to approach the problem might be to simplify it so that it resembles a definite problem that we know an algorithmic solution for. 

##### Properties of Algorithms

- Well defined problem statement
	- The problem should not be vague

- Well defined input(s) and output(s)
	- It should halt with the correct output for all possible inputs
	- It shouldn't not halt or halt with incorrect outputs for any input (within the domain)

- Well defined and finite procedure
	- Every should be definite and not rely on any infinitesimal procedure 
	- https://cs.stackexchange.com/questions/31932/what-exactly-is-an-algorithm

##### Factors used to judge Algorithms
- A problem can have many different algorithmic solutions. Depending on the circumstances certain solutions might be preferred over others.

- **Correctness:** The most important factor to judge a potential algorithmic solution to a problem is whether or not it is correct in the first place.
	- Most often there is no point in discussing algorithmic solutions that are incorrect (such solutions are thus, naturally disqualified)

- **Time Complexity:**

- **Memory Complexity:**

- The above three factors are used to judge all algorithms as they are independent of the nature of the problem or other related factors
	- The best algorithms for any particular problem tends have perform well in all these categories. 

- Depending on certain scenarios it might be beneficial to value certain other factors along with (if not more than) the above three:
	- Examples

- Factors dependent or indepedent of hardware?

- Efficiency vs Other benefits

- Best vs Approximate solution

- Stable Sorting algorithms

- NP Complete algorithms

// Reasses the factors quality of an algorithm is judged on
// Determine RAM etc requirement