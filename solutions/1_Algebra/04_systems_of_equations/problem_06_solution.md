# Exercise 6 — A System with a Parameter

## 1. Problem Statement
Analyze, depending on the parameter $a$, the system
$$\begin{cases}x+y=2,\\ax+ay=4.\end{cases}$$
Determine which of the three possibilities — exactly one solution, infinitely many solutions, no solution — actually occur and for which values of $a$. If one type cannot occur, explain why.

## 2. Method and Key Formula
The left-hand side of the second equation is $a$ times the left-hand side of the first. Compare the right-hand sides as well. Equivalently, use elimination to see whether the equations are independent, identical, or contradictory.

## 3. Detailed Step-by-Step Solution
If $a\ne0$, divide the second equation by $a$ to obtain
$$x+y=\frac4a.$$
Together with $x+y=2$, this gives a consistent system only if
$$\frac4a=2\quad\Longrightarrow\quad a=2.$$
- If $a=2$, both equations are the same equation $x+y=2$, so there are infinitely many solutions.
- If $a\ne0$ and $a\ne2$, the equations require two different values for $x+y$, so there is no solution.
- If $a=0$, the second equation becomes $0=4$, which is impossible, so there is no solution.

There is no value of $a$ that produces exactly one solution, because both equations always have proportional coefficient rows $(1,1)$ and $(a,a)$; their rank cannot be 2.

## 4. Verification and Consistency Checks
For $a=2$, every point $(x,y)=(t,2-t)$ satisfies both equations. For $a=0$, the contradiction is explicit. For any nonzero $a\ne2$, the required sums $2$ and $4/a$ differ.

## 5. Final Answer
$$\boxed{\begin{aligned}
a=2 &: \text{ infinitely many solutions},\\
a\ne2 &: \text{ no solution},\\
&\text{exactly one solution: never.}
\end{aligned}}$$