<!-- title: Stirling Numbers -->

### [<-- Back to the home page](index.md)

# Stirling Numbers of the Second Kind

$\left\{ {n \atop k} \right\}$ or S(n, k) is the number of ways of partitioning an $n$ element set into $k$ subsets.

[A008277 on the OEIS](https://oeis.org/A008277)

## Basic Recurrence
$$\left\{{ n \atop n }\right\} = 1 \quad  \text{ for } n \geq 0$$

$$\left\{{ n \atop 0 }\right\} = \left\{{ 0 \atop k }\right\} = 0 \quad \text{ for } n, k>0$$

$$\left\{{n+1\atop k}\right\} = k \left\{{ n \atop k }\right\} + \left\{{n\atop k-1}\right\}
\quad \text{ for } 0<k<n$$
## Formulas

$$\left\{ {n \atop k}\right\} = \frac{1}{k!}\sum_{i=0}^k (-1)^{k-i} \binom{k}{i} i^n = \sum_{i=0}^k \frac{(-1)^{k-i} i^n}{(k-i)!i!}$$


## Identities

$$\sum_{k=0}^n \left\{ {n \atop k} \right\}(x)_k=x^n$$

$$\left\{ {n \atop n-1}\right\} = \binom{n}{2}$$

$$\left\{ {n \atop 2}\right\} = 2^{n-1}-1$$


$$\left\{{n+1\atop k+1}\right\} = \sum_{j=k}^n {n \choose j} \left\{{ j \atop k }\right\}\\$$

$$
\left\{{n+1\atop k+1}\right\} = \sum_{j=k}^n (k+1)^{n-j} \left\{{j \atop k}\right\}\\$$

$$
\left\{{n+k+1 \atop k}\right\} = \sum_{j=0}^k j \left\{{ n+j \atop j }\right\} \\$$

$$\left\{{n \atop \ell+m } \right\} \binom{\ell+m}{\ell} = \sum_k \left\{{k \atop \ell} \right\} \left\{{n-k \atop m } \right\} \binom{n}{k}$$

## Generating functions

See [Wikipedia](https://en.wikipedia.org/wiki/Stirling_numbers_of_the_second_kind)

## Related sequences

[Associated Stirling Numbers](associatedStirling.md)

[Restricted Stirling Numbers](restrictedStirling.md)

[Bell Numbers](bellNumbers.md)
