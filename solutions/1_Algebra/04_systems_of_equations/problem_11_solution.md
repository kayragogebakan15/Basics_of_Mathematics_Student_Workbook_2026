# Exercise 11 — A Parameter in a System of Three Equations

## 1. Problem Statement
Analyze the number of solutions depending on $t$:
$$\begin{cases}x+y+z=1,\\x+ty+z=2,\\x+y+tz=3.\end{cases}$$
Use elimination and separately analyze parameter values for which a standard calculation step ceases to be valid.

## 2. Method and Key Formula
Subtract the first equation from the second and third to isolate the parameter-dependent terms. This avoids dividing by $t-1$ before checking the exceptional value $t=1$.

## 3. Detailed Step-by-Step Solution
Subtract equation 1 from equation 2:
$$(t-1)y=1.$$
Subtract equation 1 from equation 3:
$$(t-1)z=2.$$
**Exceptional case:** If $t=1$, these equations become $0=1$ and $0=2$. The system is inconsistent and has no solution.

**Non-exceptional case:** If $t\ne1$, divide by $t-1$:
$$y=\frac1{t-1},\qquad z=\frac2{t-1}.$$
Use the first equation to find $x$:
$$
x=1-y-z
=1-\frac1{t-1}-\frac2{t-1}
=1-\frac3{t-1}
=\frac{t-4}{t-1}.
$$
Thus there is exactly one solution for every $t\ne1$.

## 4. Verification and Consistency Checks
For $t\ne1$, the values satisfy equation 1 by construction. Equation 2 is obtained by adding $(t-1)y=1$ to equation 1, and equation 3 is obtained by adding $(t-1)z=2$ to equation 1. Hence all three original equations hold.

## 5. Final Answer
$$\boxed{
\begin{cases}
\text{no solution},&t=1,\\
\text{one solution }\left(\frac{t-4}{t-1},\frac1{t-1},\frac2{t-1}\right),&t\ne1.
\end{cases}}$$