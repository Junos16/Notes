#SetTheory #Logic #FoundationsofMathematics #NBGSetTheory #ZFCSetTheory 

When discussing any theory related to sets, it is important to know how sets can be created. In Naive Set Theory it was assumed that given any well-defined condition we could define a set containing all the elements that fulfill that condition. 

***Unrestricted Comprehension:*** $\exists A \forall x (x \in A \iif )$

### Paradox
- ***Russel's Paradox:*** $Let\space \Omega = \{x \mid x\notin x\} \implies (\Omega \in \Omega \iff \Omega \notin \Omega)$  
- If $\Omega$ is defined as a set that contains all sets that aren't members of themselves then we can draw the following conclusions:
	- If $\Omega$ belongs in itself then by the definition of the set $\Omega$ it satisfies the property that it does not belong in itself. Contradiction.
	- If $\Omega$ doesn't belong in itself then by the definition of set $\Omega$ is satisfies the property required to be a member of itself. Contradiction.
- Russel's Paradox arises as a consequence of the assumption made in naive set theory that any set that can be intuitively described exists. This can be formulated as follows:
	- ***Axiom of Unrestricted Comprehension:*** $\exists S \forall x (x \in S \iff \phi(x))$
- Different axiomatizations of set theory have attempted to replace this assumption with another axiom or axiom schema to 

### Resolution via ZFC Set Theory
- In ZFC, we replace Unrestricted Comprehension with Axiom of Specification. Reformulating the Russel set:
	- Let $\Omega$ be a set containing all sets $\exists A x \in A$ that satisfy the property $x \notin x$
- If $\Omega \in \Omega$ then $\Omega \in A$ and $\Omega \notin \Omega$
- If $\Omega \notin \Omega$ then $\Omega \notin A$ or $\Omega \in \Omega$
- Of all the possibilities we have 2 contradictions
- Thus we conclude without any contradiction that if A is a set then $\Omega \notin A$ 

### Resolution via NBG Set Theory
- In NBG, Unrestricted Comprehension is replaced with Class Comprehension. So reformulating the Russel set:
	- Let $\Omega$ be a class containing all sets $x$ that satisfy the property $x \notin x$
- If $\Omega \in \Omega$ then $\Omega$ is a set and $\Omega \notin \Omega$
- If $\Omega \notin \Omega$ then $\Omega$ not a set or $\Omega \in \Omega$
- Of all the possibilities we have 2 contradictions
- Thus we conclude without any contradiction that $\Omega$ is not a set 
