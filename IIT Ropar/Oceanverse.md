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

>For any $n\times n$ matrix, it is invertible iif the discriminant is 0

15. We will now see matrices as functions. Instead of $\phi$ we will write the matrix itself: $$\left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$.

>OK

16. Consider the function $$\left( \begin{matrix} 1 & 2 \\2 & 4 \\\end{matrix}\right) : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$. This matrix takes a few elements to the origin. What are those elements? Plot this using Geogebra.

>$$\begin{align}x+2y &= 0 \\ 2x+4y &= 0 \\ \implies x = -2y\end{align}$$
Thus any vector $\left(\begin{matrix}x \\ y\end{matrix}\right)$ such that $x = -2y$ satisfies the equation $$\left( \begin{matrix} 1 & 2 \\2 & 4 \\\end{matrix}\right)\left(\begin{matrix}x \\ y\end{matrix}\right)=\left(\begin{matrix}0 \\ 0\end{matrix}\right)$$
# Module B

17. $A$ is assigned $0$, $B:1$, $C:2$, and so on up to $Z:25$. Assume you denoted every letter with a number, as given in the table above. You need to encrypt the word $$SUDARSHANA$$ which stands for the numbers: $$18, 20, 3, 0, 17, 18, 7, 0, 13,0$$You encrypt this using a matrix given by : $$ \left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) $$So $SUDARSHANA$ will end up becoming: $$96, 134, 6, 9, 88, 123, 14, 21, 26, 39$$Given these numbers, how will you decrypt the message and get back $SUDARSHANA$? This is a well known cryptographic protocol called the Hill Cipher. You can read more online.

>Multiply each pair with the $A^{-1}$ where $$A= \left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right),\space A^{-1} =  \left( \begin{matrix} -4 & 3 \\3 & -2 \\\end{matrix}\right)$$This gives: $$\left( \begin{matrix} -4 & 3 \\3 & -2 \\\end{matrix}\right) \left( \begin{matrix} 96 \\ 134 \\\end{matrix}\right) = \left( \begin{matrix} 18 \\ 20 \\\end{matrix}\right)$$

18. We encounter equations very often in our lives. Consider for example, the following situation at **_Baker’s Cafe_**. The manager has a very important estimate to make. Mostly, visitors at his cafe happen to be families and they are often comprised of Children and/or Adults. He observes that there are 3 adults and 1 child at a table and their bill turns out to be Rs.1200/-. There is yet another table with 2 children and 1 adult and their bill comes out to be Rs.1000/-. Can the manager estimate the consumption of a Child/Adult? This is popularly called the _Simultaneous Equations_ and we all remember from our school days, multiple ways in which these can be solved. $$\begin{aligned}3A+1C&=1200 \\ 1A+2C&=1000 \end{aligned}$$
>$A = 100,\space C = 450$

19. While we were taught the so called two variables and two unknowns, what if there were more equations than unknowns? $$\begin{aligned}3A+1C&=1200\\1A+2C&=1000\\1A+1C&=900 \end{aligned}$$
>System is overdetermined and thus has no solution

20. Note that the previous question can be modelled as a matrix: $$\begin{aligned}3A+1C&=1200\\1A+2C&=1000\\1A+1C&=900 \end{aligned}$$ <u>Observe</u> this is the same as: $$ \left( \begin{matrix} 3 & 1 \\1 & 2 \\1 & 1 \\\end{matrix}\right) \left( \begin{matrix} A\\ C\\\end{matrix} \right) = \left(	\begin{matrix} 1200\\ 1000\\ 900\\\end{matrix} \right)$$
>Yes

21. One obvious way to solve this, is to guess the values :-). Can you get closer to the solution by guessing? Note that there is no solution to this question. You can just reduce the error. Do you see why?

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

27. What is $(x,y,z)$ satisfying the following equation? (Use Geogebra) $$\left[\begin{matrix}1 &2&3\end{matrix}\right]\left[\begin{matrix}x \\ y \\ z\end{matrix}\right]=0$$
>![[Pasted image 20240531121200.png]]

28. Use Geogebra and plot all the points in the set below. $$T={\alpha(1,2,1)|\alpha\in \mathbb{R}}$$

>![[Pasted image 20240531125601.png]]


29. Use Geogebra and plot all the points in the set below. $$S={\beta(2,7,3)|\beta\in \mathbb{R}}$$

>![[Pasted image 20240531125730.png]]

30. Use Geogebra and plot all the points in the set below. $$W={\alpha(1,2,1)+\beta(2,7,3)|\alpha,\beta\in \mathbb{R}}$$
>![[Pasted image 20240531130114.png]]


# Module D
