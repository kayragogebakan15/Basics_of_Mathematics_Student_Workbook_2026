# Exercise 14 — Rotation Matrices

## 1. Problem Statement

For
\[
R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix},
\]
compute \(R(\alpha)R(\beta)\) and show using angle-sum identities that it equals \(R(\alpha+\beta)\). Explain the geometric meaning.

## 2. Theoretical Background and Concepts

A two-dimensional rotation through angle \(\theta\) is represented by \(R(\theta)\). The trigonometric identities
\[
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
\]
\[
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta
\]
allow the product to be simplified.

## 3. Detailed Step-by-Step Solution

Multiply the matrices:
\[
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta&
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta&
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}.
\]
Using the angle-sum identities, this becomes
\[
\begin{pmatrix}
\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\
\sin(\alpha+\beta)&\cos(\alpha+\beta)
\end{pmatrix}
=R(\alpha+\beta).
\]

## 4. Verification and Consistency Checks

The result has exactly the standard form of a rotation matrix with angle \(\alpha+\beta\). For example, setting \(\beta=0\) gives \(R(\alpha)R(0)=R(\alpha)I=R(\alpha)\), consistent with the identity rotation.

## Final Answer

\[
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}.
\]
Geometrically, applying a rotation by \(\beta\) and then one by \(\alpha\) is equivalent to a single rotation by their sum.
