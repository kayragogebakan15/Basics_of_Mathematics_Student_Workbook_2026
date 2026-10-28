# Exercise 8 — Row Operations and Their Reversibility

## 1. Problem Statement

Starting with
\[
A=\begin{pmatrix}1&2&-1\\2&4&1\\-1&1&3\end{pmatrix},
\]
perform in order: (1) \(R_2\leftarrow R_2-2R_1\), (2) \(R_3\leftarrow R_3+R_1\), and (3) interchange \(R_2\) and \(R_3\). Show each matrix and give the inverse operation for each step.

## 2. Theoretical Background and Concepts

An elementary row operation changes one row by a reversible rule. Adding a multiple of another row is reversed by subtracting that multiple; swapping two rows is reversed by swapping them again.

## 3. Detailed Step-by-Step Solution

### Step 1: \(R_2\leftarrow R_2-2R_1\)

The new second row is
\[
(2,4,1)-2(1,2,-1)=(0,0,3).
\]
Thus,
\[
A_1=\begin{pmatrix}1&2&-1\\0&0&3\\-1&1&3\end{pmatrix}.
\]
Inverse operation: \(R_2\leftarrow R_2+2R_1\).

### Step 2: \(R_3\leftarrow R_3+R_1\)

The new third row is
\[
(-1,1,3)+(1,2,-1)=(0,3,2).
\]
Thus,
\[
A_2=\begin{pmatrix}1&2&-1\\0&0&3\\0&3&2\end{pmatrix}.
\]
Inverse operation: \(R_3\leftarrow R_3-R_1\).

### Step 3: Interchange \(R_2\) and \(R_3\)

\[
A_3=\boxed{\begin{pmatrix}1&2&-1\\0&3&2\\0&0&3\end{pmatrix}}.
\]
Inverse operation: interchange \(R_2\) and \(R_3\) again.

## 4. Verification and Consistency Checks

Each operation changes only the specified row or row positions. Reversing Step 1 restores row 2 because \((R_2-2R_1)+2R_1=R_2\); the same cancellation applies to Step 2. A row swap performed twice restores the original row order.

## Final Answer

\[
A_1=\begin{pmatrix}1&2&-1\\0&0&3\\-1&1&3\end{pmatrix},\quad
A_2=\begin{pmatrix}1&2&-1\\0&0&3\\0&3&2\end{pmatrix},\quad
A_3=\begin{pmatrix}1&2&-1\\0&3&2\\0&0&3\end{pmatrix}.
\]
