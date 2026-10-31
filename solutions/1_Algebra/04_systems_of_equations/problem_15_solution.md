# Exercise 15 — Classifying Three Systems

## 1. Problem Statement
For each system, perform only as much elimination as necessary to recognize its type:
1. $\begin{cases}x+y=2,\\x-y=0\end{cases}$
2. $\begin{cases}x+y=2,\\2x+2y=4\end{cases}$
3. $\begin{cases}x+y=2,\\2x+2y=5\end{cases}$
For each, justify the classification: one solution, infinitely many solutions, or no solution.

## 2. Method and Key Formula
Use one row operation to compare the equations. A pivot in both variable columns gives a unique solution. A zero row gives a redundant equation and infinitely many solutions if a free variable remains. A row $[0\ 0\mid c]$ with $c\ne0$ is a contradiction.

## 3. Detailed Step-by-Step Solution
**System 1:**
$$\left[\begin{array}{cc|c}1&1&2\\1&-1&0\end{array}\right]
\xrightarrow{R_2\leftarrow R_2-R_1}
\left[\begin{array}{cc|c}1&1&2\\0&-2&-2\end{array}\right].$$
The second row gives $y=1$, and the first then gives $x=1$. There is one solution.

**System 2:**
$$\left[\begin{array}{cc|c}1&1&2\\2&2&4\end{array}\right]
\xrightarrow{R_2\leftarrow R_2-2R_1}
\left[\begin{array}{cc|c}1&1&2\\0&0&0\end{array}\right].$$
The second equation is redundant. The remaining equation is $x+y=2$, so let $y=t$ and $x=2-t$. There are infinitely many solutions.

**System 3:**
$$\left[\begin{array}{cc|c}1&1&2\\2&2&5\end{array}\right]
\xrightarrow{R_2\leftarrow R_2-2R_1}
\left[\begin{array}{cc|c}1&1&2\\0&0&1\end{array}\right].$$
The second row represents $0=1$, so there is no solution.

## 4. Verification and Consistency Checks
For system 1, $(1,1)$ satisfies both equations. For system 2, every $(2-t,t)$ satisfies $x+y=2$ and therefore both original equations. For system 3, doubling the first equation would require $2x+2y=4$, which conflicts with $2x+2y=5$.

## 5. Final Answer
1. $\boxed{\text{One solution: }(x,y)=(1,1).}$
2. $\boxed{\text{Infinitely many solutions: }(x,y)=(2-t,t),\ t\in\mathbb R.}$
3. $\boxed{\text{No solution; the system is inconsistent.}}$