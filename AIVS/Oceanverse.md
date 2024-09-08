# Module A

1. Ram and Lakshman were two brothers, Ram's pocket money was twice as Lakshman. The good boys that Ram and Lakshman were, they did not spend their pocket money on anything. They instead saved the same in their piggy bank. Every week, they would check their savings so far. Assume the first week's savings was $(R_1,L_1)$ and second week's $(R_2,L_2)$ and so on. They try plotting their weekly savings on a graph sheet. How will the points look like?

>![[Pasted image 20240529112022.png]]

2.  Atul's house is centered at origin $(0,0)$ he walks straight (along the x-axis) for 2 units and then takes a left and walks 1 unit to reach Bala's house, after that he takes a right turn and walks for one unit and then a left turn and walks for one unit and reaches Chetan's house. He continues in a similar style, takes a right turn 1 unit and then left turn one unit and reaches Divya's house. Are the houses of Bala, Chetan and Divya on a straight line? What is the equation of this line? Plot this on Geogebra

>![[Pasted image 20240529115006.png]]

3. Plot the lines $y=x$, $y=2x$, $y=10x$.

>![[Pasted image 20240529115059.png]]

4. Observe that they all pass through the origin. Why?

>The y-intercept is $0$ since $(0,0)$ satisfies the equation

5. Plot $y=2x+1$. Observe, Why doesn't it pass through the origin?

>![[Pasted image 20240529115642.png]]
>
>y-intercept is not $0$ since $(0,0)$ doesn't satisfy the equation

6. Plot $y=ax+b$, with $a$ and $b$ as parameters which you should be able to vary. What do you observe?

>![[Pasted image 20240529115856.png]]
>
>$a$ is the slope of the equation and $b$ is the y-intercept of the equation

6. a. Let a line be $y=5x+6$. For what values of $\alpha$ and $\beta$ will the line $y= \alpha x + \beta$ be parallel to the given line? When will it intersect the given line in the 3rd quadrant?

>Parallel: For $\alpha = 5$ and any $\beta$
>
>Intersect in 3rd Quadrant: $\alpha$ and $\beta$ such that $x_{0}<0,y_{0}$<0 and $y_{0}=5x_{0}+6$ and $y_{0}=\alpha x_{0}+\beta$


7. Consider the following simultaneous equation:   $$2x+3y=7$$$$3x+4y=10$$Do you see a 2x2 matrix here? What is the importance of seeing a matrix in this problem? Why study matrices in general?<br>Do you observe that this problem can be retold as: $$\left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix} \right) \left( \begin{matrix} x\\ y\\ \end{matrix} \right) =\left( \begin{matrix} 7\\ 10\\ \end{matrix} \right)$$
>Yes
>When working with linear systems the variables often aren't significant but the coefficients are. Isolating the coefficients makes manipulation and computation simpler (example performing gaussian elimination, least square approximation) especially when the system is massive

8. Consider a simple function $f(x) = 3x+2$. This function is invertible right? Can you tell us what is $\alpha$ such that $f(\alpha)=17$? Is such an $\alpha$ unique? How did you find such an $\alpha?$. Is this always possible?

>![[Pasted image 20240529231509.png]]
>$\alpha$ here is unique since $f(x)$ here is bijective. $\alpha = f^{-1}(17)$. It is only possible if the function is bijective. 

9. Consider the function $$f(x)=x^2-10$$, what is $f(5)$?

>![[Pasted image 20240529232124.png]]

10. Consider the function $$f(x)=x^2-10$$, if $f(\alpha)=54$, what is $\alpha$?

>![[Pasted image 20240529232235.png]]

11. Consider the function $$g(x)=x^3-x^2-10x+2$$, if $g(x)=-22$ what is $x$?

>![[Pasted image 20240529232439.png]]

12. Do you know what is $\mathbb{R}, \mathbb{R}^2 and\ \mathbb{R}^3$?

>Set of all real numbers, set of all ordered pairs of real numbers, set of all ordered triples of real numbers

13. Consider the function $\phi : \mathbb{R}^2\rightarrow \mathbb{R}^2$ defined by $$\phi (x,y)=(2x+3y,3x+4y)$$. Find $x$ and $y$ such that $\phi (x,y)=(5,6)$. Observe that $(5,6)$ as well as $(x,y)$ lies in $\mathbb{R}^2$.

>![[Pasted image 20240529234530.png]]

14. Is the function $\phi$ invertible? In the question above on matrices, we see that it is of the form $A\vec{x}=b$. Note that we can invert the matrix, using the method that was taught to us in our high school to find out the value for the variables $x$ and $y$. This is one of the many applications of matrices.

>Yes. $$\phi^{-1}(x) = (-4x+3y, 3x-2y)$$
>Matrix representation $$\begin{align}\left( \begin{matrix} 2 & 3 \\3 & -4 \\\end{matrix} \right) \left( \begin{matrix} x\\ y\\ \end{matrix} \right) &=\left( \begin{matrix} 5\\ 6\\ \end{matrix} \right)\\ \left( \begin{matrix} x\\ y\\ \end{matrix} \right) &= \left( \begin{matrix} -2\\ 3\\ \end{matrix} \right)\end{align}$$
14. (a) Take a random looking $2\times2$ matrix. Is it invertible? How often is it invertible?

>For any $n\times n$ matrix, it is invertible iif the 

15. We will now see matrices as functions. Instead of $\phi$ we will write the matrix itself: $$\left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$.

>OK

16. Consider the function $$\left( \begin{matrix} 1 & 2 \\2 & 4 \\\end{matrix}\right) : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$. This matrix takes a few elements to the origin. What are those elements? Plot this using Geogebra.

>$$\begin{align}x+2y &= 0 \\ 2x+4y &= 0 \\ \implies x = -2y\end{align}$$
Thus any vector $\left(\begin{matrix}x \\ y\end{matrix}\right)$ such that $x = -2y$ satisfies the equation $$\left( \begin{matrix} 1 & 2 \\2 & 4 \\\end{matrix}\right)\left(\begin{matrix}x \\ y\end{matrix}\right)=\left(\begin{matrix}0 \\ 0\end{matrix}\right)$$
# Module B

17. $A$ is assigned $0$, $B:1$, $C:2$, and so on up to $Z:25$. Assume you denoted every letter with a number, as given in the table above. You need to encrypt the word $$SUDARSHANA$$ which stands for the numbers: $$18, 20, 3, 0, 17, 18, 7, 0, 13,0$$You encrypt this using a matrix given by : $$ \left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) $$So $SUDARSHANA$ will end up becoming: $$96, 134, 6, 9, 88, 123, 14, 21, 26, 39$$Given these numbers, how will you decrypt the message and get back $SUDARSHANA$? This is a well known cryptographic protocol called the Hill Cipher. You can read more online.

>Multiply each pair with the $A^{-1}$ where $$A= \left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right),\space A^{-1} =  \left( \begin{matrix} -4 & 3 \\3 & -2 \\\end{matrix}\right)$$This gives: $$\left( \begin{matrix} -4 & 3 \\3 & -2 \\\end{matrix}\right) \left( \begin{matrix} 96 \\ 134 \\\end{matrix}\right) = \left( \begin{matrix} 18 \\ 20 \\\end{matrix}\right)$$

18. We encounter equations very often in our lives. Consider for example, the following situation at **_Baker’s Cafe_**. The manager has a very important estimate to make. Mostly, visitors at his cafe happen to be families and they are often comprised of Children and/or Adults. He observes that there are 3 adults and 1 child at a table and their bill turns out to be Rs.1200/-. There is yet another table with 2 children and 1 adult and their bill comes out to be Rs.1000/-. Can the manager estimate the consumption of a Child/Adult? This is popularly called the _Simultaneous Equations_ and we all remember from our school days, multiple ways in which these can be solved. $$\begin{aligned}3A+1C&=1200 \\ 1A+2C&=1000 \end{aligned}$$
>$A = 280,\space C = 360$

19. While we were taught the so called two variables and two unknowns, what if there were more equations than unknowns? $$\begin{aligned}3A+1C&=1200\\1A+2C&=1000\\1A+1C&=900 \end{aligned}$$
>System is overdetermined and thus has no solution

20. Note that the previous question can be modelled as a matrix: $$\begin{aligned}3A+1C&=1200\\1A+2C&=1000\\1A+1C&=900 \end{aligned}$$ <u>Observe</u> this is the same as: $$ \left( \begin{matrix} 3 & 1 \\1 & 2 \\1 & 1 \\\end{matrix}\right) \left( \begin{matrix} A\\ C\\\end{matrix} \right) = \left(	\begin{matrix} 1200\\ 1000\\ 900\\\end{matrix} \right)$$
>Yes

21. One obvious way to solve this, is to guess the values :-). Can you get closer to the solution by guessing? Note that there is no solution to this question. You can just reduce the error. Do you see why?

>**2d Solution:**
>Intersections of the 3 equations: $(280, 360), (800, 100), (150, 750)$. The point inside a triangle that minimizes the distances between the vertices is the centroid. So required value $=(410,403.33)$ 
>**3d Solution:**
>

22. In the figure below: ![[Pasted image 20240529224836.png]] If 1000 people were to start in one state, what will be the distribution of people eventually? Write down a python script to find the convergence.

>$P(Happy|Start=Happy) = 0.4166, P(Stressed|Start=Happy) = 0.5833,$ $P(Happy|Start=Stressed) = 0.375, P(Stressed|Start=Stressed) = 0.6499$

23. In the figure below: ![[Pasted image 20240529224913.png]] If 1000 people were to start in one state, what will be the distribution of people eventually? Write down a python script to find the convergence.

>$P(Prk|Start = Prk) = 0.404, P(Apt|Start = Prk) = 0.352, P(Rst|Start = Prk) = 0.244$>$P(Prk|Start = Apt) = 0.4, P(Apt|Start = Apt) = 0.333, P(Rst|Start = Apt) = 0.267$>$P(Prk|Start = Rst) = 0.316, P(Apt|Start = Rst) = 0.492, P(Rst|Start = Rst) = 0.192$

# Module C

24. Use Geogebra: Draw the vector $\left[\begin{matrix} 1\\1\end{matrix}\right]$ Find out all those vectors which are perpendicular to this vector.
>![[Pasted image 20240531101327.png]]

25. Do you observe that we are asking for vectors $\left[\begin{matrix} x \\ y \end{matrix}\right]$ such that, $$\left[\begin{matrix}1 &1\end{matrix}\right]\left[\begin{matrix}x \\ y\end{matrix}\right]=0$$
> Vectors perpendicular to $\left[\begin{matrix}1 \\ 1\end{matrix}\right]$ lie on the line $x+y=0$. Using matrix notation: $$\left[\begin{matrix}1 &1\end{matrix}\right]\left[\begin{matrix}x \\ y\end{matrix}\right]=0$$

26. Use Geogebra and solve the above question with $\left[\begin{matrix}1 &1\end{matrix}\right]$ replaced by $\left[\begin{matrix}a &b\end{matrix}\right]$. Use $(a, b)$ as parameters and check what happens to $(x,y)$.

>![[Pasted image 20240531120730.png]]
>If $a,b\neq0$ then the only solution is $(0,0)$. If $a = 0$ then $y=0$ is the solution (any value of $x$ satisfies the equation). Same with $b$.

27. What is $(x,y,z)$ satisfying the following equation? (Use Geogebra) $$\left[\begin{matrix}1 &2&3\end{matrix}\right]\left[\begin{matrix}x \\ y \\ z\end{matrix}\right]=0$$
>![[Pasted image 20240531121200.png]]

28. Use Geogebra and plot all the points in the set below. $$T=\{\alpha(1,2,1)|\alpha\in \mathbb{R}\}$$

>![[Pasted image 20240531125601.png]]


29. Use Geogebra and plot all the points in the set below. $$S=\{\beta(2,7,3)|\beta\in \mathbb{R}\}$$

>![[Pasted image 20240531125730.png]]

30. Use Geogebra and plot all the points in the set below. $$W=\{\alpha(1,2,1)+\beta(2,7,3)|\alpha,\beta\in \mathbb{R}\}$$
![[Pasted image 20240531130114.png]]

31. In the above set $W$ find out all the points $(x,y,z)$ satisfying the following: (Use Geogebra)
$$\begin{bmatrix}w_1 & w_2 & w_3\\
\end{bmatrix}  \begin{bmatrix} x\\ y \\ z\\ \end{bmatrix}=0 $$
 where $(w_1,w_2,w_3) \in W$. Note that $w_i$s are real numbers.

>BIG QUESTION !!!!!!!!%&#*#* $\lambda(1,1,-3)$ always is orthogonal to $w\in W$ 
>what is the relevance of   $$M=\begin{bmatrix}1 & 2 & 1\\ 2 & 7 &3 \end{bmatrix}$$
>//////////////////////////////////////////////////////////////////////////////////////////////
>$$\begin{bmatrix}w_1 & w_2 & w_3\\\end{bmatrix} = \begin{bmatrix}(\alpha + 2\beta) & (2\alpha + 7\beta) & (\alpha + 3\beta) \\\end{bmatrix}$$ we have $$\begin{align}\begin{bmatrix}w_1 & w_2 & w_3\\
\end{bmatrix}  \begin{bmatrix} x\\ y \\ z\\ \end{bmatrix}&=0 \\ \implies \begin{bmatrix}(\alpha + 2\beta) & (2\alpha + 7\beta) & (\alpha + 3\beta) \\\end{bmatrix}\begin{bmatrix} x\\ y \\ z\\ \end{bmatrix}&=0 \\ \implies (\alpha + 3\beta)x  +(2\alpha + 7\beta)y + (\alpha + 3\beta)z &= 0 \\ \implies (x + 2y + z)\alpha + (3x + 7y + 3z)\beta &= 0 \end{align}$$
>![[WhatsApp Image 2024-05-31 at 20.25.30_885b874a.jpg]]

32. Given the matrix $$A=\begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix}$$, find out all the possible $(x,y,z)$ such that:
$$ \begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix} \begin{bmatrix} x\\ y\\ z\\ \end{bmatrix}=0$$
Observe carefully, what has this question got to do with previous five questions in this module

>$x = z, y = -2z$ 

33. Given the matrix $$A=\begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix}$$ what does the following three sets represent?
(i) $\mathscr{R}=\{\alpha(1,2,3) + \beta(4,5,6) + \gamma(7,8,9) |\alpha, \beta, \gamma\in \mathbb{R}\}$
(ii) $C=\{\alpha(1,4,7) + \beta(2,5,8) + \gamma(3,6,9) | \alpha, \beta, \gamma \in \mathbb{R}\}$
(iii) $N=\{(x,y,z)|x(1,4,7) + y(2,5,8) + z(3,6,9) = 0 \}$
 Use only Geogebra

>$\mathscr{R}$ rowspace. $C$ column space. $N$ null space.
>![[Pasted image 20240601182017.png]]
>![[Pasted image 20240601182106.png]]
> ![[Pasted image 20240601182958.png]]

34. Did you observe that every vector of $\mathscr{R}$ is perpendicular to every vector of $N$?

>Yes, in this case $C$ is also orthogonal to $N$

35. Consider the matrix
 $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}$$. Draw the line $2y+x=4$. Seeing the matrix $B$ as a function $B:\mathbb{R^2}\mapsto \mathbb{R^2}$, where does $B$ takes the line  $2y+x=4$? Where does it take:
		i)$2y+x=10$
		ii)$2y+x=62$
		iii)$2y+x=1800$

>$$\left[ \begin{matrix} 1 & 2 \\2 & 4 \\\end{matrix}\right]\left[\begin{matrix}x \\ y\end{matrix}\right]=\left[\begin{matrix}x+2y \\ 2x+4y\end{matrix}\right]$$
>$$\begin{align}2x+y=4 &\mapsto 4x+8y=4\\
2x+y=10 &\mapsto 4x+8y=10 \\
2x+y=62 &\mapsto 4x+8y=62 \\
2x+y=1800 &\mapsto 4x+8y=1800 \\
\end{align}$$

35. a) In general $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}:\mathbb{R^2}\mapsto \mathbb{R^2}$$, where does this function take $2y+x=k$?(where $k$ is a constant)

>$$2x+y=k \mapsto 4x+8y=k$$

36. Consider a matrix $$A=\begin{bmatrix} 1 & 4 \\ 2 & 3\\ \end{bmatrix}$$ and a vector $v$ =  $\begin{bmatrix} 1 \\ 1\\ \end{bmatrix}$ to what is it transformed?     	(a). Is it rotated?   
	(b). Is the magnitude preserved?    
	(c). What is the ratio of magnitude of $Av$ to $v$?

> (a). No
> (b). No
> (c). 5

37. Given $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}:\mathbb{R^2}\mapsto \mathbb{R^2}$$. What is the range of this function?

> All solutions are of the form $y=2x$

38. You have achieved the required wisdom if you have realized that: $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}:\mathbb{R^2}\mapsto \mathbb{R^2}$$."$B$ collapses a dimension ".

> Column vectors are of the form $a = kb$ so, linear combination can only lie on a single line (2d to 1d)

# Module D

39. Given the matrix $$M=\begin{bmatrix} 1 & 3 \\ 2 & 6\\ \end{bmatrix}$$. Use Geogebra to plot $\mathscr{R}$, $\mathscr{C}$ & $\mathscr{N}$. what do you observe?
(i) $\mathscr{R}=\{\alpha(1,3) + \beta(2,6) | \alpha, \beta\in \mathbb{R}\}$
(ii) $\mathscr{C}=\{\alpha(1,2) + \beta(3,6) | \alpha, \beta\in \mathbb{R}\}$
(iii) $\mathscr{N}=\{(x,y)| x(1,3) + y(2,6) = 0, \forall x,y\in \mathbb{R} \}$

>i) ![[Pasted image 20240601185437.png]]
>ii) ![[Pasted image 20240601185550.png]]
>iii) ![[Pasted image 20240601185619.png]]

40. Note that $\mathscr{C}$ and $\mathscr{N}$ are orthogonal.

>Yes, $\mathscr{N}$ is null space of $M^{T}$

41. What is  the null-space of $$M=\begin{bmatrix} 1 & 3 \\ 2 & 6\\ \end{bmatrix}$$ & the null-space of $M^T$?

>Null space of $M$![[Pasted image 20240601185736.png]]
>Null space of $M^{T}$![[Pasted image 20240601185619.png]]

42. Do you observe that $C(M) \perp N(M^T)$,  $R(M)\perp N(M)$ ?

> Yes

43. Consider $$A=\begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix}$$ What is $N(A), C(A), R(A), N(A^{T})$

>$N(A) = \{\lambda(1,-2,1)|\lambda\in\mathbb{R}\}$
>$C(A)=\{\alpha(1,4,7) + \beta(2,5,8) + \gamma(3,6,9) | \alpha, \beta, \gamma \in \mathbb{R}\}$
>$R(A)=\{\alpha(1,2,3) + \beta(4,5,6) + \gamma(7,8,9) |\alpha, \beta, \gamma\in \mathbb{R}\}$
>$N(A^{T}) = \{\lambda(1,-2,1)|\lambda\in\mathbb{R}\}$

44. Consider a 4x4 matrix $M$: $\mathbb{R^4}\mapsto \mathbb{R^4}$ whose range is
	a) $4-Dimension$
	b) $3-Dimension$ 
	c) $2-Dimension$
	d) $1-Dimension$
	e) $0-Dimension$
	Give an example each for all the above 5 cases.

>a)  $\begin{bmatrix}1 & 1 & 1 & 1 \\ 0 & 1 & 1 & 1\\ 0 & 0 & 1& 1\\ 0 & 0 & 0 & 1 \end{bmatrix}$
>b) $\begin{bmatrix}1 & 1 & 1 & 1 \\ 0 & 1 & 1 & 1\\ 0 & 0 & 1& 1\\ 0 & 0 & 0 & 0 \end{bmatrix}$
>c) $\begin{bmatrix}1 & 1 & 1 & 1 \\ 0 & 1 & 1 & 1\\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0 \end{bmatrix}$
>d) $\begin{bmatrix}1 & 1 & 1 & 1 \\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0 \end{bmatrix}$
>e) $\begin{bmatrix}0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0 \end{bmatrix}$

45. Consider $A : \mathbb{R^{3}} \to \mathbb{R^{3}}$
	a) Show that if the range contains a point $(a,b,c)$, then it should contain the entire set $S$, defined by: $S= \{\alpha(a, b,c)| \alpha \in \mathbb{R}\}$.
	b) Show that if the range contains the points $(a,b,c)$ and $(d,e,f)$, then the range contains the entire set $T$ defined by: $T=\{\alpha(a,b,c) + \beta(d,e,f) \thinspace|\thinspace  \alpha,\beta\in \mathbb{R}\}$.
	c) Note: $S$ is of the dimension $1$, but $T$ need'nt be of dimension $2$. Think!

>a) $T(k\vec{x})=kT(\vec{x})$
>b) $T(k_{1}\vec{x}+k_{2}\vec{x})=k_{1}T(\vec{x})+k_{2}T(\vec{x})$
>c) If the two vectors are linearly dependent on each other then the result is 1 - dimensional
# Module E

46. Give an example of two  $2-dim$ subspaces in $\mathbb{R^{3}}$. Let us call it $S_1, S_2$.

> $S_{1}:=\{(x,y,0)|x,y\in\mathbb{R}\},S_{2}:=\{(0,y,z)|y,z\in\mathbb{R}\}$

47. Let $S_3$ be all those vectors perpendicular to $S_1$. $S_4$ be that of $S_2$.

>$S_{3}:=\{(0,0,z)|z\in\mathbb{R}\},S_{4}:=\{(x,0,0)|x\in\mathbb{R}\}$

48. Find a matrix $M$ whose Null-Space is $S_3$. column space is $S_2$.

>$$M=\begin{bmatrix}0 & 0 & 0\\ 0 & 1 & 0\\ 1 & 0 & 0\\ \end{bmatrix}$$

49. What does $S_1$ and $S_4$ represent?

>

50. Do you observe there is a bijection from $S_1  \to S_2$?

>$$M=\begin{bmatrix}0 & 0 & 0\\ 1 & 0 & 0\\ 0 & 1 & 0\\ \end{bmatrix}$$
>$M$ maps $(a,b,0)$ to $(0,a,b)$. 
>The mapping is injective because if $(0,a_{1},b_{1}), (0,a_{2},b_{2})\in S_{2}$ and $(0,a_{1},b_{1}) = (0,a_{2},b_{2})$ then we can conclude by the definition of n-tuples $(a_{1},b_{1},0)=(a_{2},b_{2},0)$
>The mapping is surjective since $\forall (0,a,b)\in S_{2}$ can we show that $(a,b,0)$ is in $S_{1}$

# Module F
51. Imagine a situation of war in 1800’s. Country A wants to send a letter to Country B such that their enemy country can’t understand the message. How can you help the country A in this situation?

>Using a predefined mapping of each letter to another. Ex. map the nth alphabet to the 26-nth alphabet

52. How about shifting the alphabets by 1 letter each? What is the problem here?

>We can test 25 times to get readable text

53. Try encoding the word “VICHARANASHALA” using the above method (But shift 4 letters this time)

>ZMGLEVEREWLEPE

54. What if you have only the encoded message? How will you get to the original message?

>Test all 25 shifts, one of them gives english

55. What if we substitute each letter by some other letter using a pre- defined mapping (eg.a->t,b->f,c->y,…)?How many trails do we have to do so that we can reach the secret message if we only have the encoded text and not the mapping ?

>26!

56. Is there any efficient approach for the second part of the 55th question?

>For large enough text perform frequency analysis

57. What do you think is the frequency of occurence of various letters in a sample English text? Which letter do you expect to be the most frequent 

> frequencies = {
	'e': 0.1270, 't': 0.0906, 'a': 0.0817, 'o': 0.0751, 'i': 0.0697,
	'n': 0.0675, 's': 0.0633, 'h': 0.0609, 'r': 0.0599, 'd': 0.0425,
	'l': 0.0403, 'c': 0.0278, 'u': 0.0276, 'm': 0.0241, 'w': 0.0236,
	'f': 0.0223, 'g': 0.0202, 'y': 0.0197, 'p': 0.0193, 'b': 0.0149,
	'v': 0.0098, 'k': 0.0077, 'j': 0.0015, 'x': 0.0015, 'q': 0.0010,
	'z': 0.0007
}

58. Assuming that an English text follows a particular order of frequency, can you solve the 56th question?

>Yes

59. Suppose we take a subset from a huge text i.e kth𝑘𝑡ℎ, 2kth2𝑘𝑡ℎ, 3kth3𝑘𝑡ℎ… elements. Will they also follow the same pattern observed in the previous question?

>For a large enough text, yes

60. Assume you arrange two meaningful english text strings in front of each other. What is the expected number of collisions in the letters? Call it “collision frequency”.

>$p_{a}^{2}+p_{b}^{2}+...+p_{z}^{2}$

61. Assume that in the previous question ,we apply the ceaser cypher(the one discussed inthe first few questions), on both the strings, and alphabet by 5 letters then will the collision frequency remain the same? What if we shift first string by 3 letters and second by 5?

>$p_{d}p_{f}+p_{e}p_{g}+...+p_{c}p_{e}$

62. Suggest any such method using which we can be confident that the encoded text can’t be decoded by the enemy. (We may discuss it in further classes)

>RSA (Assymmetrical)
# Module G

63. A dart is thrown at random onto a board that has the shape of a circle as shown below. Calculate the probability that the dart will hit the shaded region. 
	![[Pasted image 20240605220036.png]]

>$$\begin{align} 
P(Shaded) &= \frac{\pi(R^{2}- r^{2})}{\pi R^{2}} \\
&=\frac{14^{2}-7^{2}}{14^{2}} \\
&= 0.75
\end{align}$$

64. Let a pair of dice be thrown and the random variable X be the sum of the numbers that appear on the two dice. Find the mean or expectation of X.

>$$\begin{align}
E(X) &= 2\left(\frac{1}{36}\right)+3\left(\frac{2}{36}\right)+...+6\left(\frac{5}{36}\right)+7\left(\frac{6}{36}\right)+8\left(\frac{5}{36}\right)+...+11\left(\frac{2}{36}\right)+12\left(\frac{1}{36}\right)
\\
E(X) &= \frac{252}{36} = 7
\end{align}$$

65. A factory produces items, and each item is independently defective with probability 0

66. If 100 items are produced in a day, what is the expected number of defective items?

>$$E(X) = \sum\limits_{i=1}^{100}i\binom{100}{i}(0.02)^{i}(0.98)^{100-i} = 2 
$$
66. A point is chosen at random inside a sphere of radius R. What is the probability that this point is closer to the center of the sphere than to its surface?

>$$\frac{\frac{4}{3}\pi\left(\frac{R}{2}\right)^3}{\frac{4}{3}\pi R^3}=\frac{1}{8}$$

67. A point is randomly chosen inside a cube with side length 𝑎. What is the probability that the point is closer to one of the vertices than to the center of the cube?

>$$P=\frac{1}{2}$$

68. Imagine you have a number line that ranges from -1 to 1. You randomly pick k points on this line. What is the expected distance of the closest point to the midpoint of the line?

>$$\frac{1}{k+1}$$
# Module H

69. Plot and find the distance between points using Geogebra: $A(1,2)$, $B(2,3)$ and $C(5,9)$

>![[Pasted image 20240610153455.png]]

70. Using Geogebra, which two points are the closest ones? What's the distance between them?

>![[Pasted image 20240610153719.png]]
>$AB=\sqrt2$

71. Add four more points: $D(0,-1)$, $E(4,11)$, $F(8,12)$, $G(-3,6)$ to your graph. What’s the closest pair now?

>![[Pasted image 20240611152924.png]]
>$AB=\sqrt2$

72. Suppose we have 10 points. How many pairs of points do you have to consider for finding the closest pair?

>$\binom{10}{2}$

73. What is the Y sorted order (by default assume ascending) of points $A$, $B$, $C$, $D$, $E$?

>DABCE

74. Plot a line $L$ parallel to the Y-axis passing through the middle point in the X sorted order of the above points. Divide the set of points into left and right regions around the line

>![[Pasted image 20240611152836.png]]

75. Find the closest pair of points in the left region and right region. What’s the minimum distance (say d) out of the two distances?

>Left: $AB = \sqrt2$
>RIght: $CE=\sqrt5$
>min = $AB = \sqrt2$ 

76. Consider a band of width 2d around the Line L. Find the closest pair in this band. Compare this distance with d, the minimum value of the corresponding closest pair of our graph. Is the answer the same as the brute-force method you applied in question 71? (This divide and conquer method is known as the closest pair algorithm).

>$AB=\sqrt2$

77. Astronomers have recorded the positions of stars in a 3D coordinate system where each star is represented as a point. Given the coordinates of stars (1,2,3), (4,5,6), (6,7,8), (10,11,12), find the closest pair of stars.(Use Geogebra).Is the closest pair algorithm valid here?

>![[Pasted image 20240611154524.png]]
>Yes

78. If $F(0) = 0$, $F(1) = 1$, $F(n) = F(n-1) + F(n-2)$ for $n \geq 2$, find the value of $F(5)$.

>5

79. Dry run and find the output of the following python code:  
```
def f(n):  
    if n == 0:  
        return 1  
    return n * f(n-1)  
print(f(5))
```

>$5! = 120$

80. Does the closest pair algorithm assume that the $x$ coordinates (and $y$ coordinates) of the points are distinct? Is there a problem with the $O(nlog(n))$ performance if they are not distinct(do we have to handle this special case seprately in our algorithm)?

>Yes, it assumes that the x coordinates (or whatever axis is chosen) is distinct. Just sorting and then finding the central values 

81. Given a set of points where most points are far apart, but a few points are very close to each other, can you develop an algorithm more efficient from our original algorithm to find the closest pair in this special case.

>ignore any points that have significantly large separation in one coordinate

# Module I

82. Do you know the idea of equally likely events? What are these? Can you think of any event which is not equally likely?

>Equally Likely Events: Probability of the events is the same
>Non-Equally Likely Events: Ex: Likelihood of a random indian person being under the poverty line

83. You are given two coins .What is the probability that one head and one tail shows up on tossing?

>1/2

84. In a class in which all students practise at least one sport, 60% of students play soccer or basketball and 10% practice both sports. If there is also 60% that do not play soccer, calculate the probability that a student chosen at random from the class:
	1. Plays soccer only.
	2. Play basketball only.
	3. Plays only one of the sports.
	4. Plays neither soccer nor basketball.

>$$\begin{align}
P(S\cup B) = 0.6, P(S\cap B) &= 0.1, P(\overline{S}) = 0.6 \\
P(S) &= 1 - 0.6 = 0.4 \\
P(S\cup B) &= P(S) + P(B) - P(S\cap B)\\
\implies P(B) - P(B\cap S) &= P(S\cup B) - P(S)\\
&= 0.6 - 0.4= 0.2 \\
P(S\cap \overline{B})+P(\overline{S} \cap B) = P(S\cup B) - P(S\cap B) &= 0.6 - 0.1 = 0.5 \\
P(\overline{S\cup B}) &= 1 - P(S\cup B) = 0.4 
\end{align}$$

85. Imagine you are writing your semester exams . To write an exam , there are 70% chances that an alarm clock will wake you up successfully. If you hear the alarm clock then there are 95% chances you will write the exam and if you don’t hear the alarm the chances are 50%. a)If you have written the exam what are the chances that you heard the alarm clock? b) What are the chances that you didn’t hear the alarm if you have not written the exam?

>$$\begin{align}P(A) = 0.7, P(E|A) &= 0.95, P(E|\overline{A}) = 0.5 \\
P(A|E) &= \frac{P(E|A)P(A)}{P(E)} \\
&= \frac{P(E|A)P(A)}{P(E|A)P(A) + P(E|\overline{A})P(\overline{A})} \\
&= \frac{0.95\times 0.7}{0.95\times0.7 + 0.5\times0.3} \\
&= 0.816 \\
P(\overline{A}|\overline{E}) &= \frac{P(\overline{E}|\overline{A})P(\overline{A})}{P(\overline{E})} \\
&= \frac{(1-P(E|\overline{A}))(1-P(A))}{1-(P(E|A)P(A) + P(E|\overline{A})P(\overline{A}))} \\
&= \frac{0.5\times 0.3}{1-(0.95\times0.7 + 0.5\times0.3)} \\
&= 0.811 
\end{align}$$

86. Lets say an investment company “Future Wealth“ analyses stocks and predicts whether their price will go up or down. So far, half of the stocks analysed by the company have gone up, 3/4 of the stocks that went up were correctly predicted to go up, and 2/5 of the stocks that went down were incorrectly predicted to go up. Suppose that the company tells you that it will go up. Compute the probability that the stock will indeed go up.

>$P(U)=0.5,P(U|u)=0.75,P(D|u)=0.2$

87. Imagine you are a bettor. You are watching a race between two horses A and B. Let’s say five races are conducted. Construct any three hypotheses defining winning probabilities of A and B. What confidence do you have in each of your hypotheses to be true? Lets say , out of 5 races A wins 3 and B wins the remaining 2 (AAABB). Then after 5 races , in which of your hypotheses will you have maximum confidence. As per your new hypothesis which horse has more chances to win the 6th round .

>Hypothesis: 1) A>B := 3/5, A=B, A<B,

88. You’re training a spam filter . You have data on the frequency of certain words in both spam and non-spam emails. How would you update your beliefs about an email being spam or not spam based on the presence of specific words?Let’s say initially chances of an email being spam is 40%. Data: Word “free” appears in 80% of spam emails and 5% of non-spam emails

>Probability of spam $P(S) = 0.4$. Probabilities of presence of word "free" $P(F|S) = 0.8, P(F|\overline{S}) = 0.05$. Updating belief using Bayes's Theorem: 
$$\begin{align}
P(S|F) &= \frac{P(F|S)P(S)}{P(F|S)P(S) + P(F|\overline{S})P(\overline{S})} \\
&= \frac{0.8\times0.4}{0.8\times0.4 + 0.05\times0.6} \\
&= 0.914
\end{align}$$

89. Suppose that we use a perceptron to detect spam messages. Let’s say that each email message is represented by the frequency of occurrence of keywords, and the output is +1 if the message is considered spam.  
	a) Can you think of some keywords that will end up with a large number of positive weight in the perceptron?  
	b)How about keywords that will get a negative weight?  
	c)What parameters in the perceptron directly affects how many border-line messages end up being classified as spam?

>a) free, discount, offer
>b) 
>c) activation function

90. Lets have some parameters 3.1, 4.2 and 4 and the corresponding weights 5,1,and 3 respt. Calculate the weighted sum.

>$31.7$

91. Suppose you have set of numbers ranging from -infinity to infinity. Will it be easy to plot them in a limited screen size and compare them?

>no, normalize the range of the numbers

92. Will simply dividing them by some large number work?

>hard to visualize to high overlap

93. Can you think of a way to fit these numbers in some finite range? Think about some kind of functions?

>sigmoid function, relu, tanh

# Module J

94. Write the number 25 in its binary form.

>11001

95. Given a text data, how will you convert it into binary form?

>Convert to ascii then convert to binary

96. What if we use the binary code for each character according to the ASCII convention? How much space would each character take up?

>7 bit + 1 parity bit

97. Suppose I take the following notation for the letters s, o, n, h and a:
	s: 00
	o: 001
	a: 010
	h: 011
	n: 1
Decode the following string: ‘00011010110011’

>Ambiguous due to the variation in lengths. 00, 011, 010, 1, 1, (00, 1, 1) or (001, 1)

98. Do you observe that the above string can have 2 different interpretations?

>Shannsnn or Shannon

99. Can this issue occur if we take each code of the same length? Can you define one such coding for the above example, i.e., s, o, n, h and a? At least how many digits would you have to take for each character?

>s(000), o(001), n(010), h(011), a(100)

100. Observe that for 5 unique letters, I cannot have unique binary representations if I take length of each notation _exactly 2_. Why?

>5th letter would have the same representation as the first one if we follow a consistent pattern

101. Suppose you go to buy apples. There are three varieties of apples available. Your mom has given you a task that you have to buy 2 apples of any one type, 3 of the any other type, and 5 of the third. How will you minimise the total money spent?

>Costs: $c_{1}<c_{2}<c_{3}$ then optimal solution is: $5c_{1}+3c_{2}+2c_{3}$

102. Given the text ‘this is a new experience’. Write the frequency distribution of these characters for this sentence.

>t: 1, h: 1, i: 3, s: 2, (space): 4, a: 1, n: 2, e: 4, w: 1, x: 1, p: 1, r: 1, c: 1

103. To which characters should I give a shorter notation as compared to the others?

>(space) and e to reduce the length the most

104. Do you observe that the issue occurred in fifth question was because the code of ‘s’ is a prefix of the code for ‘o’?

>Yes

105. What all do you think should be the properties of a proper encoding rule?

>Unambiguous encoding, one-to-one mapping, equal length encoding

106. Get some quite basic knowledge about trees as data structures.

>Ok

107. Observe that the lower is a node in a tree, the more is the time you would take to reach till it from the top node.

>Yes
# Module K

108. In a huge network of webpages, how does the browser decides which webpage should be appeared on top?

>Filter them by search keywords and sort by most popularity

109. Read about the Algorithms Random Walk and Equal points Distribution and try to figure out how they are able to find the importance of the webpages?

>Equal Points distribution allots equal probabilities for user to start at a web page. Random Walk gives us the eventual probabilities of user landing on other web pages after multiple iterations

110. Are you able to visualize that the Equal points distribution method is nothing but a repetitive matrix operation on a vector?

>Yes

111. Will the points of the webpages calculated the Equal points distribution method converge? If yes how can you be sure about it?

>Some web pages will have multiple incoming links from other very popular web pages, those would be the web pages where the population would converge to.
>
>In terms of the transition matrix $(T)$ we can express it after eigendecomposition as follows: 
>$$\begin{align}
T&=PEP^{-1} \\
T^{n}&=PE^{n}P^{-1} \\
\end{align}$$Since all the eigenvalues are less than 1, we know that $E$ converges

112. Is this convergence dependent on the initial vector?

>No

113. If you have three websites, A, B, and C, and all are linked to each other, what happens to the importance of each website if:  
	Website A is linked to by both B and C.  
	B is linked to by A.  
	C is linked to by A.  
	How does the number of links pointing to a website affect its perceived importance?

>

114. Given 4 buckets (A, B, C, and D):  
	A passes its coins to B and C  
	B passes its coins to D  
	C passes its coins to A  
	D passes its coins to B  
	If each bucket starts with 1 coin, calculate the number of coins in each bucket after first round and second round.

>

115. In both the algorithms (Random Walk and Equal Distributions) what problem would you face if we have some highly connected nodes? Would it affect the evaluation of other nodes?

>

116. What modifications in the algorithm can you think to solve this problem?

>

![[Pasted image 20240708155409.png]]
# Module L

117. How does a computer represent an image? (Hint: pixels)

>Approximately represented using a matrix of pixels

118. Are you able to relate this with matrices? If yes, then is this matrix invertible?

>Some of the columns of the matrix might be very similar but due to small errors and variations, it might lead to invertibility (for small images this might not be the case, or for block color backgrounds, for large and complex enough images the matrix is guaranteed to be invertible)

119. Given a 2X2 matrix, what is the probability that the matrix is non-invertible?

>Very low

120. What would happen if I randomly remove one pixel form it, would it make any change? What about removing two, three, four… pixels?

>For big enough images, it won't make a difference

121. How many pixels you can remove in this way? When would you stop?

>We could reduce the resolution in each step of the reduction, 

122. Can we retrieve the removed pixels?

>

123. How much difference do you expect in two adjacent pixels in an image?



124. Can you think of a systematic way of removing pixels from the image?



125. Can you retrieve the removed pixels back in this way?

# Module M

126. Recall linear transformation that you studied in previous modules. What do they do?



127. Let a vector $v=[3,4]$ and matrix be $A= [[1/ \sqrt{2},-1/ \sqrt{2}],[1/ \sqrt{2},1/ \sqrt{2}]]$, find A, what do you observe?



128. Let a vector $v=[3,4]$ and matrix be $B= [[ \sqrt{3}/2,-1/2],[1/2,\sqrt{3}/2]]$ find Bv, what do you observe?



129. What similarity can you observe in matrix A and B?



130. Let a vector $b=[3,4]$  and a matrix $D=[[2,0],[0,3]]$ find Db. Can you observe that the matrix D simply scaled the respective axis of the vector?



131. Are you aware of orthogonal matrices? What properties do orthogonal matrices show?



132. What is the relation between transpose and inverse of an orthogonal matrix?



133. What do you get when you multiply $A$ and $A^T$?



134. Find the eigen vectors of $AA^T$ for different matrices A, and find the common feature in these eigen vectors.



135. Observe what does a matrix $A =[[1,0],[0,1],[0,0]]$ do when applied to a vector in $R^2$.



136. Observe what does a matrix $A =[[1,0,0],[0,1,0]]$ do when applied to a vector in $R^3$.

# Module N

137. What do you understand by convolution? Suppose we have two sets $(A)$ and $(B)$: $A = \{1, 2, 3, 4\} , B = \{5, 6, 7, 8\}$. What is $A \ast B$ ? And what about  $B \ast A$? Are they the same? 

>$$\begin{align}
A \ast B &= \{A_{1}\cdot B_{1}, A_{1}\cdot B_{2} + A_{2}\cdot B_{1}, A_{1}\cdot B_{3} + A_{2}\cdot B_{2} + A_{3}\cdot B_{1}, A_{1}\cdot B_{4} + A_{2}\cdot B_{3} + A_{3}\cdot B_{2} + A_{4}\cdot B_{1}, A_{2}\cdot B_{4} + A_{3}\cdot B_{3} + A_{4}\cdot B_{2}, A_{3}\cdot B_{4} + A_{4}\cdot B_{3}, A_{4}\cdot B_{4}\} \\ &= \{5, 16, 34, 60, 61, 52, 32\}
\end{align}$$

138. How do you convolve two matrices? Let two matrices be A and B. A=$$ \left( \begin{matrix} 3 & 1 &-1 \\1 & 2 &0 \\1 & 1 & 8 \\\end{matrix}\right) $$ and B = $$ \left( \begin{matrix} 1 & 0 & -1\\4 & -2 & 0 \\6 & 5 & 1 \\\end{matrix}\right) $$ then what is $A \ast B$?

>If $C = A\ast B$ then $C_{ij}=\sum\limits_{r}\sum\limits_{k}A_{rk}B_{(i-r,j-k)}$

139. What is the purpose of using filters on images?
# Module O
