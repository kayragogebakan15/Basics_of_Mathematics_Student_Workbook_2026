# Exercise 8 — Two Systems with the Same Coefficient Matrix

## 1. Problem Statement
Solve by elimination:
$$\begin{cases}2x+y=5,\\x-y=1,\end{cases}
\qquad
\begin{cases}2x+y=1,\\x-y=4.\end{cases}$$
Compare the successive elimination steps. Which part is the same in both cases, and why?

## 2. Method and Key Formula
Write each augmented matrix and eliminate one variable. The coefficient matrix is the same in both systems, so the coefficients used in elimination are the same; only the right-hand-side arithmetic changes.

## 3. Detailed Step-by-Step Solution
For the first system:
$$\left[\begin{array}{cc|c}2&1&5\\1&-1&1\end{array}\right].$$
Use $R_1\leftarrow R_1-2R_2$:
$$\left[\begin{array}{cc|c}0&3&3\\1&-1&1\end{array}\right],$$
so $3y=3$, hence $y=1$. From $x-y=1$, $x=2$.

For the second system:
$$\left[\begin{array}{cc|c}2&1&1\\1&-1&4\end{array}\right].$$
Use the same row operation $R_1\leftarrow R_1-2R_2$:
$$\left[\begin{array}{cc|c}0&3&-7\\1&-1&4\end{array}\right],$$
so $3y=-7$, hence $y=-\frac73$. From $x-y=4$,
$$x=4+y=4-\frac73=\frac53.$$

## 4. Verification and Consistency Checks
First solution: $2(2)+1=5$ and $2-1=1$. Second solution:
$$2\left(\frac53\right)-\frac73=1,\qquad \frac53-\left(-\frac73\right)=4.$$
The row operation on the coefficient columns is identical in both systems because the coefficient matrix is unchanged. Only the transformed right-hand side differs.

## 5. Final Answer
$$\boxed{(x,y)=(2,1)\text{ for system 1},\qquad
(x,y)=\left(\frac53,-\frac73\right)\text{ for system 2}.}$$