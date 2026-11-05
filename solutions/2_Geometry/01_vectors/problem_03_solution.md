# Exercise 3 — Vector Normalization

## 1. Problem Statement
For $v=(3,4)$ find a unit vector $e$ with the same direction and orientation. Check that $\|e\|=1$, reconstruct $v$ in the form $v=\|v\|e$, and explain what changes during normalization and what remains unchanged.

## 2. Method and Key Formula
A unit vector in the direction of a nonzero vector $v$ is obtained by dividing by its length:
$$e=\frac{v}{\|v\|}.$$
This changes the length to $1$ but preserves direction and orientation.

## 3. Detailed Step-by-Step Solution
First calculate the length:
$$\|v\|=\sqrt{3^2+4^2}=\sqrt{9+16}=5.$$
Divide each component by $5$:
$$e=\frac15(3,4)=\left(\frac35,\frac45\right).$$

## 4. Verification and Consistency Checks
Check the unit length:
$$
\|e\|=\sqrt{\left(\frac35\right)^2+\left(\frac45\right)^2}
=\sqrt{\frac9{25}+\frac{16}{25}}=\sqrt1=1.
$$
Reconstruct the original vector:
$$
\|v\|e=5\left(\frac35,\frac45\right)=(3,4)=v.
$$
The positive scalar factor preserves the direction and orientation; only the magnitude changes from $5$ to $1$.

## 5. Final Answer
$$\boxed{e=\left(\frac35,\frac45\right),\qquad \|e\|=1,\qquad v=5e.}$$