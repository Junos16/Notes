## Maximizing Monotonic Functions

Monotonic functions always have limits at $\pm \infty$, either finite or $\pm \infty$ (Proof WIP). Thus to maximize a monotonic function we maximize or minimize $x$ if the function is increasing or decreasing (respectively). 

If a monotonically increasing function has a finite limit at $+ \infty$ then it is bounded from above
	**Proof by contradiction:** Let $\forall y>x \space f(y)\ge f(x)$) and $lim_{x \to \infty}f(x) = M$. We need to show that $\forall x M\geq f(x)$. Let us assume that $f(x)$ is not bounded from above by $M$. $\implies \exists k \ni f(k) \ge M$. Since $f(x)$ is monotonically increasing $\implies \forall x > k \space f(x)\ge f(k)$. Let $\epsilon = |f(k)-M|$. $\because \forall x > k \space f(x)\ge f(k)$ there exists no such $c \ni \forall x > c \space |f(x)-M|<|f(k)-M|$.
