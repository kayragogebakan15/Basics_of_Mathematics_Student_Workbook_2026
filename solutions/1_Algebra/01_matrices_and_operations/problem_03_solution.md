# Exercise 3 — When Can Matrices Be Multiplied?

## 1. Problem Statement

The matrix sizes are
\[
A_{2\times3},\quad B_{3\times4},\quad C_{4\times2},\quad D_{2\times2}.
\]
Determine whether each of \(AB, BA, BC, CB, AC, CA, AD, DA\) is defined and give the result size when it is defined.

## 2. Theoretical Background and Concepts

If \(X\) is \(m\times n\) and \(Y\) is \(p\times q\), the product \(XY\) is defined exactly when \(n=p\), meaning the number of columns of the first factor equals the number of rows of the second. The product then has size \(m\times q\). Order matters.

## 3. Detailed Step-by-Step Solution

| Product | Dimension check | Defined? | Result size |
|---|---|---|---|
| \(AB\) | \((2\times3)(3\times4)\): inner dimensions \(3=3\) | Yes | \(2\times4\) |
| \(BA\) | \((3\times4)(2\times3)\): \(4\ne2\) | No | — |
| \(BC\) | \((3\times4)(4\times2)\): inner dimensions \(4=4\) | Yes | \(3\times2\) |
| \(CB\) | \((4\times2)(3\times4)\): \(2\ne3\) | No | — |
| \(AC\) | \((2\times3)(4\times2)\): \(3\ne4\) | No | — |
| \(CA\) | \((4\times2)(2\times3)\): inner dimensions \(2=2\) | Yes | \(4\times3\) |
| \(AD\) | \((2\times3)(2\times2)\): \(3\ne2\) | No | — |
| \(DA\) | \((2\times2)(2\times3)\): inner dimensions \(2=2\) | Yes | \(2\times3\) |

## 4. Verification and Consistency Checks

For each defined product, the shared inner dimension disappears and the outer dimensions determine the answer size. For example, \(CA\) has outer dimensions 4 and 3, so its result is \(4\times3\). The reverse product \(AC\) is not defined because its inner dimensions do not match.

## Final Answer

Defined: \(AB\) (\(2\times4\)), \(BC\) (\(3\times2\)), \(CA\) (\(4\times3\)), and \(DA\) (\(2\times3\)). The other four products are undefined.
