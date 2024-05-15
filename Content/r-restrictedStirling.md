<!-- title: r-Stirling Numbers -->

### [<-- Back to the home page](index.md)

# r-Stirling Numbers of the Second Kind
$$\left\{
\begin{matrix}
    n\\
    k
\end{matrix}
\right\}_{r}$$
is the number of ways of partitioning the set $\{1, 2, ..., n\}$ into $k$ subsets such that $\{1, 2, ..., r\}$ are in different blocks.



## Recurrence

The r-Stirling numbers of the Second Kind follow the same recurrence as the normal Stirling Numbers of the Second Kind, but with different starting parameters.

$$\left\{
\begin{matrix}
    n\\
    k
\end{matrix}
\right\}_{r} = 0 \quad \text{ for } n < r$$

$$\left\{
\begin{matrix}
    n\\
    k
\end{matrix}
\right\}_{r} = 1 \quad \text{ for } n = m = r$$

$$\left\{{n\atop k}\right\}_r = k \left\{{ n-1 \atop k }\right\} + \left\{{n-1\atop k-1}\right\}
\quad \text{ for } n > r$$

Extra:

$$\left\{{n\atop k}\right\}_r = \left\{{n\atop k}\right\}_{r-1} - (r - 1)\left\{{n-1\atop k}\right\}_{r-1}
\quad \text{ for } n \geq r \geq 1$$

## Formulas

This formula is from Broder's article (linked below). There might be more formulas in it, and maybe in the OEIS entries too.

$$\left\{ {n \atop m} \right\}_r = \sum_k \binom{n-r}{k} \left\{ {k \atop m-r} \right\} r^{n-r-k}
$$



https://math.stackexchange.com/questions/4371769/range-of-r-parameter-of-second-kind-r-stirling-numbers
 gives:

$$\left\{ {n \atop k} \right\}_r = \sum_{i=0}^{n} \binom{n}{i} \left\{ {i \atop k} \right\} r^{n-i}$$

Be careful that there might be a mismatch in notation. It seems that the formula above produces 
$$\left\{ {n+r \atop k+r} \right\}_r = (...)$$
## Identities

$$\left\{{n\atop n}\right\}_r = 1 \text{ for } n \geq r$$
$$\left\{{n\atop m}\right\}_r = 0 \text{ for } m > n$$
$$\left\{{n\atop r}\right\}_r = r ^{n - r} \text{ for } n \geq r$$




## Generating functions

There may be some errors from copying these functions from the original paper. The notation for falling/rising factorials isn't too clear. See the article below for the originals.

#### Exponential generating function

$$\sum_k \left\{ {k+r \atop m+r} \right\}_r \frac{z^k}{k!} =
\begin{cases}
\frac{1}{m!} e^{rz} (e^z - 1)^m, & \text{if } m \geq 0, \\
0, & \text{otherwise}.
\end{cases}$$

#### Ordinary generating functions

$$\sum_k \left\{ {k \atop m} \right\}_r z^k =
\begin{cases}
\frac{z^m}{(1-rz)(1-(r+1)z) \cdots (1-mz)}, & \text{if } m \geq r \geq 0, \\
0, & \text{otherwise}.
\end{cases}$$

$$\sum_k \left\{ {n+r \atop k+r} \right\}_r x^{\underline{k}} = (x+r)^n, \quad n \geq 0.
$$

#### Double generating function

$$
\sum_{k,m} \left\{ {k+r \atop m+r} \right\}_r \frac{z^k}{k!} t^m = \exp(t(e^z - 1) + rz).
$$

## Articles
[Anderi Broder: The r-Stirling numbers](https://www.sciencedirect.com/science/article/pii/0012365X84901614)
