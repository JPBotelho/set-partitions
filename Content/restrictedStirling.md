<!-- title: Restricted Stirling Numbers -->

### [<-- Back to the home page](index.md)

# Restricted Stirling Numbers of the Second Kind
$\left\{
\begin{matrix}
    n\\
    k
\end{matrix}
\right\}
_{\le m}$ 

is the number of ways of partitioning an $n$ element set into $k$ subsets such that each subset has **at most $m$ elements**. They are often called **"Restricted Stirling numbers"** or **"r-Restricted Stirling numbers"**. 

Case m=2: https://oeis.org/A144299

Case m=3: https://oeis.org/A111246

Case m=4: https://oeis.org/A144644

Case m=5: https://oeis.org/A151509

Case m=6: https://oeis.org/A151511
## Basic Recurrence


$\left\{
\begin{matrix}
    n\\
    0
\end{matrix}
\right\}
_{\le m}
= \left\{
\begin{matrix}
    0\\
    n
\end{matrix}
\right\}
_{\le m}
= 0 \text{ for } n > 0$ 

$\left\{
\begin{matrix}
    0\\
    0
\end{matrix}
\right\}
_{\le m}
= 1$


$$
\left\{ {n+1 \atop k} \right\}_{\leq m} = \sum_{i=0}^{m-1} \binom{n}{i} \left\{ {n-i \atop k-1} \right\}_{\leq m}
$$
$$
= k \left\{ {n \atop k} \right\}_{\leq m} + \binom{n}{k-1} - \binom{n}{m} \left\{ {n-m \atop k-1} \right\}_{\leq m}
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
_{\le h}
= 0 \text{ for } n > k*h$



## Generating functions

### Exponential generating function

$$
\sum_{n=k}^{mk} \left\{ {n \atop k} \right\}_{\leq m} \frac{x^n}{n!} = \frac{1}{k!} \left( E_{m}(x) - 1 \right)^k
$$
$$
E_m(t) = \sum_{k=0}^{m} \frac{t^k}{k!}
$$

## Relation to associated stirling numbers

$$
\left\{ {n \atop k} \right\}_{\leq \infty} = \left\{ {n \atop k} \right\}_{\geq 1} = \left\{ {n \atop k} \right\}
$$

## Related sequences

[Associated Stirling Numbers](associatedStirling.md)

[Restricted Bell Numbers](restrictedBell.md)

## Sources
[Incomplete poly-Bernoulli numbers associated with incomplete Stirling numbers
](https://arxiv.org/abs/1510.05799)



