We might often be interested in creating collections of lists that contain elements taken from other collections in an orderly fashion. If we want a collection of lists with size N, then we might take N different collections such that each position of the lists only contains elements from its corresponding collection.

***Example:*** A unique card in a 52 card deck can be described by the suit and the rank of the card. We can use ordered pairs to model each card. (Heart, 3) completely describes a distinct card in a deck. We are using 2 different collections to generate all possible combinations of these pairs, the collections of all ranks $\{A, 2, 3, ..., Q, K\}$ and the collections of all suits $\{Spades, Hearts, Clubs, Diamonds\}$. We can count a total of $13 \times 4$ elements in this deck. 

Intuitively this operation is a similar to taking a product of both the collections. In set theory a cartesian product is used to model this operation. [Link test](Ordered%20N-Tuples.md)

***Cartesian Product:*** $(a,b) \in A \times B \iff (a \in A) \land (b \in B)$  

We can show that cartesian product of two sets are sets as well. 

If we want the resulting set to contain N-tuples instead of pairs, we can define the notion of N-fold cartesian product. 

***N-fold Cartesian Product:*** 