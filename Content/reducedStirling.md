<!-- title: Reduced Stirling Numbers -->

### [<-- Back to the home page](index.md)

# Reduced Stirling numbers of the second kind

$$S^d(n, k)$$
is the number of ways of partitioning the set $\{1, 2, ..., n\}$ into $k$ subsets such that in each subset, elements have pairwise distance at least $d$.

The case $d = 1$ gives the regular [Stirling numbers of the second kind](stirlingNumbers.md).


## Recurrence
$$S^d(1, 1) = 1$$
$$S^d(1, 0) = 0 \text{ for } n \geq 2$$
$$S^d(n, k) = 0 \text{ for } k \geq n$$

$$S^d(n, k) = S^d(n-1, k-1) + (k - d + 1) * S^d(n-1, k) \text{ for } n \geq k \geq d$$



## Formula

$$S^d(n, k) = S(n - d + 1, k - d + 1) \text{ for } n \geq k \geq d$$
where $S(n, k)$ is a regular Stirling number of the second kind. 


## Articles

[Applications of Chromatic Polynomials Involving Stirling Numbers](https://web.archive.org/web/20200331142047/http://www.austinmohr.com/work/files/stirling.pdf)