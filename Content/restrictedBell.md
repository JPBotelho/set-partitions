<!-- title: Restricted Bell numbers -->



### [<-- Back to the home page](index.md)

# Restricted Bell Numbers

$B_{n\leq m}$ is the number of partitions of an $n$ element set such that every block in any partition contains at most $m$ elements.

- General case: https://oeis.org/A229223

- Case m=2: https://oeis.org/A000085

- Case m=3: https://oeis.org/A001680

- Case m=4: https://oeis.org/A001681

- Case m=5: https://oeis.org/A110038

- Case m=6: https://oeis.org/A148092

- Case m=7: https://oeis.org/A229224

- Case m=8: https://oeis.org/A229225

- Case m=9: https://oeis.org/A229226

- Case m=10: https://oeis.org/A229227

## Basic Recurrence
$$B_{0 \leq m} = 1$$

$$B_{n \leq m} = B_n \text{ for } m >= n$$

$$B_{n+1 \leq m}=\sum_{k=0}^{m-1} \binom{n}{k} B_{n-k \leq m}$$



## Formulas

There is no known formula for the general case.

$$
B_{n \leq 2} = \sum_{j=0}^{\left\lfloor \frac{n}{2} \right\rfloor} \binom{n}{2j} \frac{(2j)!}{2^j j!}
$$

$$
B_{n \leq 3} = \sum_{i=0}^{\left\lfloor \frac{n}{3} \right\rfloor} \sum_{j=0}^{\left\lfloor \frac{n}{2} \right\rfloor} \binom{n}{3i} \frac{(3i)!}{6^i i!} \binom{n-3i}{2j} \binom{2j}{j} \frac{j!}{2^j}
$$
## Generating functions

### Exponential generating function

$$\sum_{n=0}^\infty \frac{B_{n \leq m}}{n!} x^n = exp(\sum_{i=1}^{m} \frac{x^i}{i!})$$

## Relation to Bell and Associated Bell numbers
Where $B_n$ is a [Bell number](bellNumbers.md) and $B_{n \geq m}$ is an [Associated Bell Number](associatedBell.md)

$$B_n = \sum_{i=0}^{n}\binom{n}{i} * B_{i\le m} * B_{n-i\ge m+1}$$

$$
B_{n \geq k} = B_{n} - \sum_{i=1}^{n} \binom{n}{i} B_{i \leq k-1} B_{n-i \geq k}.
$$
 
## Articles
[Combinatorial and Arithmetical Properties of the Restricted and Associated Bell and Factorial Numbers
](https://arxiv.org/abs/1707.08138)