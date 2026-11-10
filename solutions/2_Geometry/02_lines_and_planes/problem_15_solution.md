# Exercise 15 — Complete Classification of a Line Relative to a Plane

## 1. Problem Statement
For $L:p+tv$ and $\Pi:n\cdot X=d$, state conditions for a unique intersection, strict parallelism and containment. Illustrate each with a simple numerical example.

## 2. Theoretical Background and Concepts
Assume $v\ne0$ and $n\ne0$, so these define a genuine line and plane. Substituting the parametric line into the plane gives a scalar linear equation:

$$
n\cdot(p+tv)=d\quad\Longleftrightarrow\quad (n\cdot v)t=d-n\cdot p.
$$

Its coefficient and right-hand side determine whether it has one solution, none or infinitely many.

## 3. Detailed Step-by-Step Solution
**Case A — Unique intersection.** If $n\cdot v\ne0$, divide by the nonzero coefficient to obtain

$$
t=\frac{d-n\cdot p}{n\cdot v}.
$$

Example: $L:(x,y,z)=(0,0,1)+t(0,0,-1)$ and $\Pi:z=0$. Here $n=(0,0,1)$, $d=0$, $n\cdot v=-1$ and $n\cdot p=1$. Consequently $t=(0-1)/(-1)=1$ and the intersection is $(0,0,0)$.

**Case B — Parallel with no common points.** If $n\cdot v=0$ but $n\cdot p\ne d$, the equation becomes $0=d-n\cdot p$ with a nonzero right-hand side, which is impossible. Example: $L:(x,y,z)=(0,0,1)+t(1,0,0)$ and $\Pi:z=0$. Here $n\cdot v=0$, while $n\cdot p=1\ne0=d$.

**Case C — Line contained in the plane.** If $n\cdot v=0$ and $n\cdot p=d$, substitution gives $0=0$ for every $t$, so every line point belongs to the plane. Example: $L:(x,y,z)=(0,0,0)+t(1,0,0)$ and $\Pi:z=0$. Here both dot-product tests equal $0=d$.

## 4. Verification and Consistency Checks
For the first example, the line has $z=1-t$, which vanishes only when $t=1$. For the second example, $z=1$ for every $t$, so it never meets $z=0$. For the third, $z=0$ for every $t$, so all line points lie on the plane. These exhaust all possibilities because either $n\cdot v$ is nonzero or it is zero; in the latter case, either $n\cdot p=d$ or not.

## 5. Final Answer
A single intersection occurs when $n\cdot v\ne0$; strict parallelism occurs when $n\cdot v=0$ and $n\cdot p\ne d$; containment occurs when $n\cdot v=0$ and $n\cdot p=d$.
