**Three Prisoners Problem:** 
	- Three prisoners, A, B, and C, are in separate cells and sentenced to death. The governor has selected one of them at random to be pardoned. The warden knows which one is pardoned, but is not allowed to tell. Prisoner A begs the warden to let him know the identity of one of the two who are going to be executed. "If B is to be pardoned, give me C's name. If C is to be pardoned, give me B's name. And if I'm to be pardoned, secretly flip a coin to decide whether to name B or C." 
	- The warden tells A that B is to be executed. Prisoner A is pleased because he believes that his probability of surviving has gone up from 1/3 to 1/2, as it is now between him and C. Prisoner A secretly tells C the news, who reasons that A's chance of being pardoned is unchanged at 1/3, but he is pleased because his own chance has gone up to 2/3. Which prisoner is correct?

**Solution A:**
	Named = B $\implies$ Pardoned = C or A. So $P(C\space is\space pardoned) = P(A\space is\space pardoned) = 0.5$
	Named = C $\implies$ Pardoned = B or A. So $P(B\space is\space pardoned) = P(A\space is\space pardoned) = 0.5$

**List of Cases:**
	1. $P(A\space pardoned,\space B\space named) = (\frac{1}{3})\left(\frac{1}{2}\right) = \frac{1}{6}$
	2. $P(A\space pardoned,\space C\space named) = (\frac{1}{3})\left(\frac{1}{2}\right) = \frac{1}{6}$
	3. $P(B\space pardoned,\space C\space named) = \frac{1}{3}$
	4. $P(C\space pardoned,\space B\space named) = \frac{1}{3}$
	- Either B or C being named when A is pardoned is independent of the likelihood of A being pardoned. 
	- If C is named then we

**Problem with Solution A:**
	- The prisoner named when A is pardoned is not determined in the same way as when B or C are pardoned
	-  If B is named then $P(C\space is\space pardoned) = 1$ w
	- Thus $P(C\space is\space pardoned) \neq P(A\space is\space pardoned)$ when B is named

**Solution 2:**
	If A is pardoned then the warden names B or C (as the pardoned) by flipping a coin. So $P(B\space named|A\space is\space pardoned) = P(C\space named|A\space is\space pardoned) = 0.5$. 
	If 
