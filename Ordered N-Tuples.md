**

When we talk about lists of elements, we are interested in ‘where’ an element occurs in that list in relation to the other members of that list. Unlike sets (replace), in lists there is a notion of first, last, next and previous element. We might also be interested in how many times an element occurs in that list. Ordered N-tuples are used to model such lists in mathematics for a list of size N. 

  

Example: The fibonacci sequence goes as follows: $(0, 1, 1, 2, 3, 5, 8, 13, 21, …)$. We cannot use a set to describe this sequence. On top of just whether the numbers belong to the sequence, we are interested in the relative position of each number in the sequence. We are interested in knowing what the predecessor to 5 in the sequence is. Also we have two instances of 1 in the sequence which isn’t something that makes sense in the context of sets where we only care about whether 1 is in the set or not.

  

// Simpler example, contrast with set

  

To define an ordered n-tuple, its definition must satisfy the basic property that two lists can be equal if and only if every element in corresponding positions in both lists are equal, i.e. the 1st element of both lists must be equal, the 2nd of both must be equal, so on and so forth. 

  

We could introduce a new undefined notion of order to define ordered n-tuples, but we preferably would want to avoid having too many undefined notions in our theory. Preferably we would want to define them using sets that we know can be demonstrated to exist. 

  

We will first define an ordered pair and then use that definition to generalize to n-tuples. The most popular definition of ordered pairs is given by Kuratowski

// Confirm

  

Kuratowski’s Definition of Ordered Pair: $(a, b) = \{\{a\}, \{a, b\}\}$

  

This definition must satisfy the property that for two pairs $(a, b)$ and $(c, d)$

  

// Proof

  

(a, b) != (b, a)

**