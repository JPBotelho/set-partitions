<!-- title: Bell numbers -->



### [<-- Back to the home page](index.md)

# Bell Numbers

$B_n$ is the number of set partitions of an $n$ element set.

[A000110 on the OEIS](https://oeis.org/A000110)



## Basic Recurrence
$B_0$ = 1

$B_{n+1}=\sum_{k=0}^{n} \binom{n}{k} B_k$


#### Spivey 2008:

$B_{n+m} = \sum_{k=0}^n \sum_{j=0}^m \left\{{m\atop j}\right\} {n \choose k} j^{n-k} B_k$


## Formulas

$B_n=\frac{1}{e}\sum_{k=0}^\infty \frac{k^n}{k!}$

$B_{n}=\sum_{k=1}^{n}\frac{k^{n}}{k!}\sum_{j=0}^{n-k}\frac{(-1)^{j}}{j!}$

$B_n=\sum_{k=0}^n \left\{{n\atop k}\right\}$

where $\left\{{n\atop k}\right\}$ is a [Stirling Number of the second kind](stirlingNumber.md)


## Generating functions

### Exponential generating function

$B(x) = \sum_{n=0}^\infty \frac{B_n}{n!} x^n = e^{e^x-1}$

## Software

https://rosettacode.org/wiki/Bell_numbers
 
## Articles
https://en.wikipedia.org/wiki/Bell_number
## Blog posts

Talks about computing bell numbers efficiently.
https://fredrikj.net/blog/2015/08/computing-bell-numbers/