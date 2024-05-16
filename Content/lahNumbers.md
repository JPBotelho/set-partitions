<!-- title: Lah Numbers -->

### [<-- Back to the home page](index.md)

# Lah numbers

$$L(n, k)$$
is the number of ways of partitioning the set $\{1, 2, ..., n\}$ into $k$ ordered subsets.

https://oeis.org/A008297

https://oeis.org/A271703

Row sums: https://oeis.org/A000262
## Recurrence
$$
L(0, 0) = 1
$$
$$
L(n, k) = 0 \text{ for } n < k
$$
$$
\begin{align*}
L(n+1, k) &= (n + k) * L(n, k) + L(n, k - 1)\\
&= k (k+1) *L(n, k + 1) + 2k * L(n, k) + L(n, k - 1)
   
\end{align*}
$$

## Formula

$$
L(n, k) = \binom{n-1}{k-1} \frac{n!}{k!} = \binom{n}{k} \frac{(n-1)!}{(k-1)!} = \binom{n}{k} \binom{n-1}{k-1} (n-k)!
$$

$$
L(n, k) = \frac{n!(n-1)!}{k!(k-1)!} \cdot \frac{1}{(n-k)!} = \left(\frac{n!}{k!}\right)^2 \frac{k}{n(n-k)!}
$$

$$
k(k+1)*L(n, k+1) = (n-k)*L(n, k), \text{ for } k > 0.
$$

## Generating Functions

### Exponential Generating Function
$$\sum_{n\geq k} L(n,k)\frac{x^n}{n!} = \frac{1}{k!}\left( \frac{x}{1-x} \right)^k$$


## Reference

[Wikipedia - Lah Numbers](https://en.wikipedia.org/wiki/Lah_number)
