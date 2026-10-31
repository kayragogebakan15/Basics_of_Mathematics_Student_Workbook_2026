# Exercise 14 — A System of Equations and the Determinant

## 1. Problem Statement

Consider \(Ax=b\), where
\[
A=\begin{pmatrix}1&2\\k&4\end{pmatrix}.
\]
For which values of \(k\) does the system have exactly one solution for every \(b\)? For the remaining value, give one right-hand side \(b\) that yields infinitely many solutions and one that yields no solution.

## 2. Method and Key Formula

A square linear system \(Ax=b\) has exactly one solution for every right-hand side \(b\) if and only if \(A\) is invertible. For a \(2\times2\) matrix, invertibility is equivalent to a nonzero determinant.

## 3. Detailed Step-by-Step Solution

Calculate the determinant:
\[
\det A=1\cdot4-2\cdot k=4-2k.
\]
The matrix is invertible when
\[
4-2k\neq0\quad\Longleftrightarrow\quad k\neq2.
\]
Therefore, for every \(k\neq2\), the system has exactly one solution for every \(b\).

The exceptional case is \(k=2\). The system then becomes
\[
\begin{cases}
x_1+2x_2=b_1,\\
2x_1+4x_2=b_2.
\end{cases}
\]
The left side of the second equation is twice the left side of the first. For consistency, we must have \(b_2=2b_1\).

**Example with infinitely many solutions:** choose
\[
b=\begin{pmatrix}1\\2\end{pmatrix}.
\]
The second equation is twice the first, so both equations reduce to
\[
x_1+2x_2=1.
\]
There are infinitely many solutions, for example \(x_1=1-2s,\ x_2=s\) for any real \(s\).

**Example with no solution:** choose
\[
b=\begin{pmatrix}1\\3\end{pmatrix}.
\]
The equations would require
\[
x_1+2x_2=1,\qquad 2x_1+4x_2=3.
\]
Doubling the first equation gives \(2x_1+4x_2=2\), which contradicts the second equation requiring that same expression to equal 3. Hence there is no solution.

## 4. Verification and Consistency Checks

At \(k=2\), the determinant is \(4-2(2)=0\), so the matrix is singular. The two example right-hand sides demonstrate the two possible outcomes for a singular system: infinitely many solutions when the equations are consistent, or no solution when they are inconsistent.

## 5. Final Answer

\[
\boxed{k\neq2}
\]
For \(k=2\), \(b=(1,2)^T\) gives infinitely many solutions, while \(b=(1,3)^T\) gives no solution.