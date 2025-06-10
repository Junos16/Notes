# Ordered Field

On top of being a field with a total order defined for its elements the Reals (as well as Rationals) are also an Ordered Field

***Ordered Field:*** A field $F (F, +, \times)$ with a total ordering $(>)$ is an ordered field when the following hold:

- $\forall x, y, z \in F y > z \implies x + y > x + z$
- $\forall x, y \in F x > 0 \cap y > 0 \implies x\times y > 0$

***Proposition (Properties of an Ordered Field):*** For an ordered field $F$ the following are true:

1. $\forall x \in F x > 0 \implies 0 > (-x)$
2. $\forall x, y, z \in F x > 0 \cap y > z \implies xy > xz$
3. $\forall x, y, z \in F 0 > x \cap y > z \implies xz > xy$
4. $\forall x \in F x \neq 0 \implies x^{2} > 0$
5. $\forall x, y \in F y > x > 0 \implies \frac{1}{x} > \frac{1}{y} > 0$
6. $\forall x, y \in F y > x > 0 \implies y^{2} > x^{2}$$
7.

***Proof:***

1. $x > 0 \implies x + (-x) > (-x) \implies 0 > (-x)$
2. $x > 0 \cap y > z \implies x > 0 \cap y + (-z) > 0 \implies x(y + (-z)) > 0 \implies xy + x(-z) > 0 \implies xy - xz > 0 \implies xy > xz$
3. $0 > x \cap y > z \implies (-x) > 0 \cap y + (-z) > 0 \implies (-x)(y + (-z)) > 0 \implies (-x)y + (-x)(-z) > 0 \implies -(xy) + xz > 0 \implies xz > xy$
4.
