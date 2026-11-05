# Exercise 15 — Comparing Directions Using the Cosine of the Angle

## 1. Problem Statement
Given
$$a=(1,2,1),\qquad b=(2,4,2),\qquad c=(2,0,3).$$
For each pair, compute
$$\frac{u\cdot v}{\|u\|\,\|v\|}.$$
Order the pairs by increasing angle between the vectors. Explain why for $a$ and $b$ the value is $1$ even though the vectors have different lengths.

## 2. Method and Key Formula
The cosine of the angle between nonzero vectors is
$$\cos\theta=\frac{u\cdot v}{\|u\|\,\|v\|}.$$
Because cosine decreases on $[0,\pi]$, a larger cosine corresponds to a smaller angle. The expression depends on direction, not on positive changes in vector length.

## 3. Detailed Step-by-Step Solution
First calculate the lengths:
$$\|a\|=\sqrt{1+4+1}=\sqrt6,$$
$$\|b\|=\sqrt{4+16+4}=\sqrt{24}=2\sqrt6,$$
$$\|c\|=\sqrt{4+0+9}=\sqrt{13}.$$

**Pair $(a,b)$:**
$$a\cdot b=1\cdot2+2\cdot4+1\cdot2=12,$$
$$\frac{a\cdot b}{\|a\|\|b\|}=\frac{12}{\sqrt6\cdot2\sqrt6}=\frac{12}{12}=1.$$

**Pair $(a,c)$:**
$$a\cdot c=1\cdot2+2\cdot0+1\cdot3=5,$$
$$\frac{a\cdot c}{\|a\|\|c\|}=\frac5{\sqrt6\sqrt{13}}=\frac5{\sqrt{78}}.$$

**Pair $(b,c)$:**
$$b\cdot c=2\cdot2+4\cdot0+2\cdot3=10,$$
$$\frac{b\cdot c}{\|b\|\|c\|}=\frac{10}{2\sqrt6\sqrt{13}}=\frac5{\sqrt{78}}.$$

## 4. Verification and Consistency Checks
Since $b=2a$ with a positive scalar, the vectors point in exactly the same direction, so their angle is $0^\circ$ and their cosine is $1$. The other two cosine values are equal, so the angles between $(a,c)$ and $(b,c)$ are equal. Numerically, $5/\sqrt{78}\approx0.566$, which is less than $1$, so both angles are larger than $0^\circ$.

## 5. Final Answer
$$\boxed{
\cos\theta_{(a,b)}=1,\qquad
\cos\theta_{(a,c)}=\cos\theta_{(b,c)}=\frac5{\sqrt{78}}.
}$$
The increasing-angle order is
$$\boxed{(a,b)\text{ first, followed by }(a,c)=(b,c)\text{ (equal angles).}}$$