<!-- title: r-Bell Numbers -->

### [<-- Back to the home page](index.md)

# r-Bell Numbers
$$B_{n, r}$$
is the number of ways of partitioning the set $\{1, 2, ..., n + r\}$ such that $\{1, 2, ..., r\}$ are in different blocks.

They are the sum of the [r-Stirling numbers of the second kind](r-restrictedStirling.md), but take care about notation, as some places consider partitions of the set \{1, 2, ..., n + r\} (like this page) and others of the set \{1, 2, ..., n\} (like the stirling page). 

$$
B_{n,r} = \sum_{k=0}^{n} \left\{ \begin{matrix} n + r \\ k + r \end{matrix} \right\}_r
$$

$$
B_n = B_{n, 0}
$$

The main source of this page is the article linked below. A lot of the theorems were given for r-Bell polynomials, and I tried to translate them to r-Bell numbers. In case some formula here is giving wrong results, please see the original!

- Case r=2: https://oeis.org/A005493

- Case r=3: https://oeis.org/A005494

- Case r=4: https://oeis.org/A045379

## Recurrence

$$B_{n, r} = 0 \text{ for } n < r$$
$$B_{n, r} = 1 \text{ for } n = r$$

$$
B_{n,r} = r B_{n-1,r} + \sum_{k=0}^{n-1} \binom{n-1}{k} B_{n-1-k,r}
$$

Extra:

$$
B_{n,r} = r B_{n-1,r} + B_{n-1,r+1}
$$


## Formulas

$$
B_{n,r} = \frac{1}{e} \sum_{k=0}^{\infty} \frac{(k + r)^n}{k!}
$$

$$
B_{n,r} = \sum_{k=0}^{n} \left( \sum_{i=0}^{n} \binom{n}{i} \left\{ \begin{matrix} i \\ k \end{matrix} \right\} r^{n-i} \right)
$$

$$
B_{n,r} = \frac{2n!}{\pi e} \Im \int_{0}^{\pi} e^{e^{i\theta}} e^{re^{i\theta}} \sin(n\theta) \, d\theta.
$$


## Identities

$$
B_{n+m,r} = \sum_{j=0}^{m} \left\{ \begin{matrix} m + r \\ j + r \end{matrix} \right\}_r B_{n,r+j}.
$$

$$
B_{n,r+m} = \sum_{j=0}^{m} (-1)^{m-j} \left[ \begin{matrix} m + r \\ j + r \end{matrix} \right]_r B_{n+j,r}.
$$

This one might be wrong, as it refers to the polynomials and I tried to adapt it to just the numbers. Check the article just in case.

$$
B_{n,r} = \sum_{k=0}^{n} r^k \binom{n}{k} B_{n-k}
$$




## Generating functions
#### Exponential generating function
$$
\sum_{n=0}^{\infty} B_{n,r} \frac{z^n}{n!} = e^{(e^z-1)+rz}
$$





## Articles
[Istvan Mezo: The r-Bell Numbers
](https://cs.uwaterloo.ca/journals/JIS/VOL14/Mezo/mezo9.pdf)
