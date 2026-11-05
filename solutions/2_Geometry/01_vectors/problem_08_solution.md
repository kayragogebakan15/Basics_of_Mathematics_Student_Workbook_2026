# Exercise 8 — Linear Combination and Checking the Result

## 1. Problem Statement
Check whether $w=(5,1)$ can be written as
$$w=au+bv,$$
where $u=(1,1)$ and $v=(2,-1)$. If so, find $a,b$, reconstruct $w$ from them, and explain the geometric meaning of the existence of such coefficients.

## 2. Method and Key Formula
A vector equation is equivalent to equality of corresponding components. Thus $au+bv=w$ gives a linear system for the unknown scalars $a$ and $b$.

## 3. Detailed Step-by-Step Solution
Substitute the vectors:
$$a(1,1)+b(2,-1)=(5,1).$$
Equating components gives
$$\begin{cases}a+2b=5,\\a-b=1.\end{cases}$$
Subtract the second equation from the first:
$$3b=4\quad\Longrightarrow\quad b=\frac43.$$
Use $a-b=1$:
$$a=1+b=1+\frac43=\frac73.$$

## 4. Verification and Consistency Checks
Reconstruct the vector:
$$
\begin{aligned}
au+bv
&=\frac73(1,1)+\frac43(2,-1)\\
&=\left(\frac73,\frac73\right)+\left(\frac83,-\frac43\right)\\
&=\left(\frac{15}3,\frac33\right)=(5,1)=w.
\end{aligned}
$$
The coefficients exist, so $w$ lies in the span of $u$ and $v$. Geometrically, it can be formed by scaling and adding the two given directions.

## 5. Final Answer
$$\boxed{a=\frac73,\qquad b=\frac43,\qquad w=\frac73u+\frac43v.}$$