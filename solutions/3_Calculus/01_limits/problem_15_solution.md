# Exercise 15 — Observation Versus Proof

## 1. Problem Statement
Choose one sequence and one function from this exercise set. Evaluate the sequence for increasingly large indices and the function at arguments approaching its limit point from the left and right. Sketch both behaviors, compare observations with analytical results, and explain why finitely many numerical checks or a sketch are not proofs.

## 2. Theoretical Background and Concepts
A sequence $a_n$ converges to $L$ when, for every $\varepsilon>0$, some $N$ ensures $|a_n-L|<\varepsilon$ for all $n>N$. A function $f(x)$ has limit $L$ at $x=a$ when, for every $\varepsilon>0$, some $\delta>0$ ensures $|f(x)-L|<\varepsilon$ whenever $0<|x-a|<\delta$ in its domain. These definitions involve all sufficiently large indices or all sufficiently close arguments, not just a finite sample.

We choose the rational sequence from Exercise 1 and the removable-singularity function from Exercise 7. Their proposed limits are $2$ and $2$, respectively.

## 3. Detailed Step-by-Step Solution

### A. Sequence — Exercise 1

Consider

$$
a_n=\frac{4n^2-3n+1}{2n^2+5n-7},\qquad n\ge2.
$$

Compute several terms:

| $n$ | $a_n$ (approximately) |
|---|---:|
| $2$ | $1.000000$ |
| $5$ | $1.264706$ |
| $10$ | $1.526749$ |
| $100$ | $1.937296$ |
| $1000$ | $1.993524$ |

The values suggest convergence toward $2$. A qualitative sketch of points $(n,a_n)$ is:

~~~text
a_n
2.0 |                         .  .  . --> 2
1.8 |                    .
1.6 |              .
1.4 |         .
1.2 |      .
1.0 |  .
    +------------------------------------> n
       2    5    10         100    1000
(Spacing and height are schematic, not to scale.)
~~~

Prove the limit algebraically by dividing numerator and denominator by $n^2$:

$$
a_n=\frac{4-\frac3n+\frac1{n^2}}{2+\frac5n-\frac7{n^2}}
\longrightarrow\frac42=2.
$$

For an explicit error check, subtract the proposed limit:

$$
a_n-2=\frac{-13n+15}{2n^2+5n-7}.
$$

For $n\ge2$, the denominator is positive and at least $2n^2$. Moreover $|-13n+15|\le13n+15\le21n$, so

$$
|a_n-2|\le\frac{21n}{2n^2}=\frac{21}{2n}\longrightarrow0.
$$

Given any $\varepsilon>0$, taking $N>\max(2,21/(2\varepsilon))$ makes $|a_n-2|<\varepsilon$ for every $n>N$, establishing convergence rather than just suggesting it.

### B. Function — Exercise 7

Consider

$$
f(x)=\frac{x^2-4x+3}{x-3},\qquad x\ne3.
$$

Evaluate at points approaching $3$ from both sides:

| Side | $x$ | $f(x)$ |
|---|---:|---:|
| Left | $2.9$ | $1.9$ |
| Left | $2.99$ | $1.99$ |
| Left | $2.999$ | $1.999$ |
| Right | $3.001$ | $2.001$ |
| Right | $3.01$ | $2.01$ |
| Right | $3.1$ | $2.1$ |

The values approach $2$ from below and above. The graph is the straight line $y=x-1$ with the point $(3,2)$ removed:

~~~text
 y
 ^                         /
 |                       /
2|---------------------o---------  hole at (3,2)
 |                   /
 |                 /
 +-----------------|--------------> x
                   3
~~~

For every $x\ne3$, factor and cancel the common nonzero factor:

$$
f(x)=\frac{(x-1)(x-3)}{x-3}=x-1.
$$

Therefore

$$
\lim_{x\to3}f(x)=\lim_{x\to3}(x-1)=2.
$$

For a direct limit-definition check, observe that for $x\ne3$,

$$
|f(x)-2|=|(x-1)-2|=|x-3|.
$$

For any $\varepsilon>0$, choosing $\delta=\varepsilon$ ensures that $0<|x-3|<\delta$ implies $|f(x)-2|<\varepsilon$. This applies to both sides of $3$.

## 4. Verification and Consistency Checks
For the sequence, the tabulated values agree with the exact formulas: at $n=2$, $a_2=(16-6+1)/(8+10-7)=11/11=1$; at $n=10$, $a_{10}=371/243\approx1.526749$. The error bound proves that every sufficiently late term is close to $2$, not only the sampled ones.

For the function, $f(2.99)=1.99$ and $f(3.01)=2.01$, matching the canceled formula. The function is still undefined at $3$; this does not prevent a limit. The exact identity $|f(x)-2|=|x-3|$ proves the two-sided limit independently of the finite table.

A finite table or sketch cannot prove a universal limit statement: an unsampled sequence could change behavior after the last listed index, and a function could behave differently at points closer to its target than any listed values. The algebraic transformations and quantified error estimates address these possibilities for the specific objects chosen.

## 5. Final Answer
The selected sequence converges to $2$, and the selected function has a two-sided limit of $2$ as $x\to3$ despite being undefined at that point. Numerical tables and sketches support the conclusions; the algebraic and error-bound arguments establish them.
