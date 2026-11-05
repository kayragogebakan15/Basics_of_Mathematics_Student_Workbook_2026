# Exercise 5 — Angle Between Vectors

## 1. Problem Statement
Given $u=(1,1,0)$ and $v=(1,0,1)$:
1. Use the sign of $u\cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

## 2. Method and Key Formula
For nonzero vectors, the angle $\theta\in[0,\pi]$ satisfies
$$\cos\theta=\frac{u\cdot v}{\|u\|\,\|v\|}.$$
For nonzero vectors, the sign of the dot product gives this classification. If $u\cdot v>0$, then $0^\circ\leq\theta<90^\circ$: the endpoint $0^\circ$ is a zero angle, and the other cases are acute. If $u\cdot v=0$, then $\theta=90^\circ$ and the angle is right. If $u\cdot v<0$, then $90^\circ<\theta\leq180^\circ$: the endpoint $180^\circ$ is a straight angle, and the other cases are obtuse. The angle is undefined if either vector is zero.

## 3. Detailed Step-by-Step Solution
First calculate the dot product:
$$u\cdot v=1\cdot1+1\cdot0+0\cdot1=1.$$
Since it is positive, the angle is expected to be acute.

The vector lengths are
$$\|u\|=\sqrt{1^2+1^2+0^2}=\sqrt2,\qquad
\|v\|=\sqrt{1^2+0^2+1^2}=\sqrt2.$$
Therefore,
$$\cos\theta=\frac1{\sqrt2\sqrt2}=\frac12.$$
Hence,
$$\theta=\arccos\left(\frac12\right)=60^\circ=\frac\pi3.$$

## 4. Verification and Consistency Checks
The computed angle $60^\circ$ is between $0^\circ$ and $90^\circ$, so it is acute. This agrees with the positive dot product.

## 5. Final Answer
$$\boxed{\theta=60^\circ=\frac\pi3\text{ radians (acute).}}$$