> You left your socks somewhere in your room. You think there's a 4/5 chance that they've been tossed into some random drawer of your dresser, so you start looking through your dresser's 8 drawers. After checking 6 drawers at random, you haven't found your socks yet. What is the probability you will find your socks in the next drawer you check?

$$\begin{align}
P(D) &= 0.8 \\
P(D) &= \sum\limits_{i=1}^{8}P(D_{i}) \\
\end{align}$$
Say after searching first drawer we find it to be empty. We update $P(D)$ accordingly.
$$\begin{align}
P(D|E) &= \frac{P(E|D)P(D)}{P(E|D)P(D)+P(E|\overline{D})P(\overline{D}))} \\
&= \frac{\frac{7}{8}\times 0.8}{\frac{7}{8}\times 0.8 + 1\times 0.2} \\
&\approx 0.778
\end{align}$$
After second search if drawer found to be empty:
$$\begin{align}
P(D|E_{2}) &= \frac{P(E_{2}|D)P(D)}{P(E_{2}|D)P(D)+P(E_{2}|\overline{D})P(\overline{D}))} \\
&= \frac{\frac{6}{8}\times 0.8}{\frac{6}{8}\times 0.8 + 1\times 0.2} \\
&= 0.75
\end{align}$$
After finding 6 drawers to be empty:
$$\begin{align}
P(D|E_{6}) &= \frac{P(E_{6}|D)P(D)}{P(E_{6}|D)P(D)+P(E_{6}|\overline{D})P(\overline{D}))} \\
&= \frac{\frac{2}{8}\times 0.8}{\frac{2}{8}\times 0.8 + 1\times 0.2} \\
&= 0.5
\end{align}$$

