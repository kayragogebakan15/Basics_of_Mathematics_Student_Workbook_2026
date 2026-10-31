# Exercise 12 — Homogeneous System

## 1. Problem Statement
Solve
$$\begin{cases}x+2y-z=0,\\2x+4y-2z=0,\\x-y+2z=0.\end{cases}$$
Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## 2. Method and Key Formula
A homogeneous system has the form $Ax=0$. The zero vector always satisfies it because $A0=0$. Use elimination to find any additional solutions and express free variables with parameters.

## 3. Detailed Step-by-Step Solution
The augmented matrix is
$$\left[\begin{array}{ccc|c}1&2&-1&0\\2&4&-2&0\\1&-1&2&0\end{array}\right].$$
Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:
$$\left[\begin{array}{ccc|c}1&2&-1&0\\0&0&0&0\\0&-3&3&0\end{array}\right].$$
Swap rows 2 and 3 and divide the new second row by $-3$:
$$\left[\begin{array}{ccc|c}1&2&-1&0\\0&1&-1&0\\0&0&0&0\end{array}\right].$$
The second row gives $y-z=0$, so $y=z$. Let $z=t$, hence $y=t$. The first row gives
$$x+2t-t=0\quad\Longrightarrow\quad x=-t.$$

## 4. Verification and Consistency Checks
Substitute $(x,y,z)=(-t,t,t)$:
$$-t+2t-t=0,$$
$$2(-t)+4t-2t=0,$$
$$-t-t+2t=0.$$
All equations hold for every real $t$. At $t=0$, the zero vector is included.

## 5. Final Answer
$$\boxed{(x,y,z)=t(-1,1,1),\quad t\in\mathbb R.}$$