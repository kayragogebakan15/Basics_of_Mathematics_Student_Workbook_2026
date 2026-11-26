# Exercise 2 — A Parabola from the Perspective of the Derivative

## 1. Problem Statement
For $f(x)=x^2-4x+1$, find its minimum using the derivative. Compare the answer with the vertex form and explain why both approaches give the same point.

## 2. Theoretical Background and Concepts
A critical point occurs where $f'=0$. A derivative changing from negative to positive marks a minimum. For an upward-opening quadratic, completing the square yields a vertex form $(x-h)^2+k$ whose minimum is $k$ at $x=h$.

## 3. Detailed Step-by-Step Solution
Differentiate:

$$
f'(x)=2x-4=2(x-2).
$$

Solve $f'(x)=0$ to obtain $x=2$. The derivative is negative for $x<2$ and positive for $x>2$, so the function first decreases and then increases. Evaluate:

$$
f(2)=2^2-4(2)+1=4-8+1=-3.
$$

Thus $(2,-3)$ is the global minimum point.

Complete the square independently:

$$
\begin{aligned}
x^2-4x+1
&=x^2-4x+4-4+1\\
&=(x-2)^2-3.
\end{aligned}
$$

Since $(x-2)^2\ge0$ for all real $x$, the smallest possible value is $-3$, reached only when $x-2=0$.

## 4. Verification and Consistency Checks
The second derivative is $f''(x)=2>0$, confirming upward convexity. The derivative zero and the vertex both select the symmetry axis $x=2$. Sample values $f(1)=-2$ and $f(3)=-2$ are equal and greater than $-3$, confirming symmetry about that axis.

## 5. Final Answer
The global minimum is $-3$ at $x=2$, the vertex $(2,-3)$; both methods agree because the derivative vanishes at the symmetry center of an upward-opening parabola.
