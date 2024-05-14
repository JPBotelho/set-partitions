<!-- title: Associated Stirling Numbers -->

### [<-- Back to the home page](index.md)

# Associated Stirling Numbers of the Second Kind
$\left\{
\begin{matrix}
    n\\
    k
\end{matrix}
\right\}
_{\ge m}$ 

is the number of ways of partitioning an $n$ element set into $k$ subsets such that each subset has at least $m$ elements. They are often called **"associated stirling numbers"** or **"r-associated stirling numbers"**. 

Case m=2: https://oeis.org/A008299

Case m=3: https://oeis.org/A059022

Case m=4: https://oeis.org/A059023
 
Case m=5: https://oeis.org/A059024

Case m=6: https://oeis.org/A059025

## Basic Recurrence


$\left\{
\begin{matrix}
    n\\
    0
\end{matrix}
\right\}
_{\ge m}
= \left\{
\begin{matrix}
    0\\
    n
\end{matrix}
\right\}
_{\ge m}
= 0 \text{ for } n > 0$ 

$\left\{
\begin{matrix}
    0\\
    0
\end{matrix}
\right\}
_{\ge m}
= 1$


$$
\left\{ {n+1 \atop k} \right\}_{\geq m} = \sum_{i=m-1}^n \binom{n}{i} \left\{ {n-i \atop k-1} \right\}_{\geq m}
$$
$$
= k \left\{ {n \atop k} \right\}_{\geq m} + \binom{n}{m-1} \left\{ {n-m+1 \atop k-1} \right\}_{\geq m}
$$


## Formulas

No explicit formula to calculate these numbers is known. If you find one, please let me know!


## Identities


$\left\{
\begin{matrix}
    n\\
    k
\end{matrix}
\right\}
_{\ge h}
= 0 \text{ for } n < k*h$



## Generating functions

### Exponential generating function

$$
\sum_{n=mk}^{\infty} \left\{ {n \atop k} \right\}_{\geq m} \frac{x^n}{n!} = \frac{1}{k!} \left( e^x - E_{m-1}(x) \right)^k
$$
$$
E_m(t) = \sum_{k=0}^{m} \frac{t^k}{k!}
$$

## Relation to restricted stirling numbers

$$
\left\{ {n \atop k} \right\}_{\leq \infty} = \left\{ {n \atop k} \right\}_{\geq 1} = \left\{ {n \atop k} \right\}
$$

## Related sequences

[Restricted Stirling Numbers](restrictedStirling.md)

[Associated Bell Numbers](associatedBell.md)

## Sources
[Incomplete poly-Bernoulli numbers associated with incomplete Stirling numbers
](https://arxiv.org/abs/1510.05799)


[L. Comtet, Advanced Combinatorics, Reidel, 1974, p. 222.](https://archive.org/details/Comtet_Louis_-_Advanced_Coatorics/page/n115/mode/2up)

