<!-- title: Restricted Bell numbers -->



### [<-- Back to the home page](index.md)

# Associated Bell Numbers

$B_{n\leq m}$ is the number of partitions of an $n$ element set such that every block in any partition contains at least $m$ elements.


## Basic Recurrence
The recurrence given here seems hard to compute. Consider computing [Associated Stirling Numbers](associatedStirling.md) and adding them for all $k \in \{1...n\}$. 

$$B_{0 \geq m} = 1$$

$$B_{n \geq m} = 0 \text{ for } m > n > 0$$

$$
B_{n, \geq k} = B_{n, \geq k-1} - \sum_{i=1}^{\left\lfloor \frac{n}{k-1} \right\rfloor} \frac{n!}{(k-1)!i!(n-(k-1)i)!} B_{n-(k-1)i, \geq k}.
$$

## Formulas

There is no known formula for the general case.

## Generating functions

### Exponential generating function

$$
\sum_{n=0}^{\infty} \frac{B_{n \geq m} x^n}{n!} = \exp \left( \exp(x) - \sum_{i=0}^{m-1} \frac{x^i}{i!} \right)
$$

## Relation to Bell and Associated Bell numbers
Where $B_n$ is a [Bell number](bellNumbers.md) and $B_{n \leq m}$ is a [Restricted Bell Number](restrictedBell.md)

$$B_n = \sum_{i=0}^{n}\binom{n}{i} * B_{i\le m} * B_{n-i\ge m+1}$$

$$
B_{n \geq k} = B_{n} - \sum_{i=1}^{n} \binom{n}{i} B_{i \leq k-1} B_{n-i \geq k}.
$$

$$
\sum_{i=0}^{n} \binom{n}{i} B_{i \geq 2} = B_{n}.
$$

$$B_n = B_{n \geq 1}$$
 
## Articles
[Combinatorial and Arithmetical Properties of the Restricted and Associated Bell and Factorial Numbers
](https://arxiv.org/abs/1707.08138)