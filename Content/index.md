<!-- title: Set Partitions -->

# Set partitions

In this website are resources on counting set partitions and related structures.

It is not a complete reference. These are just some of the things I learned about when studying this topic. I made this website because it would've been of great help to me. 

There might be mistakes, double check with the given sources when in doubt.

 If there is something you feel should be added, removed or changed, contact me at jpbotelho.costa (at) gmail.com

## Number of partitions

- With no restrictions [**(Bell Number)**](bellNumbers.md)

- With at least $k$ elements per block [**-> associated Bell number**](associatedBell.md)
  - With at least $k$ elements per block, and the largest block has exactly $j$ elements [**-> stackoverflow**](https://math.stackexchange.com/questions/1078391/counting-set-partitions-with-constraints)
- With at most $k$ elements per block [**-> restricted Bell number**](restrictedBell.md)
- Such that the first $k$ elements are in separate blocks [**-> r-Bell number**](r-bell.md)

- Such that elements with pairwise distance $<d$ are in separate blocks [**(reduced Bell number)** ](reducedBell.md)


- Such that the blocks are ordered but the elements in them aren't [**-> ordered Bell / Fubini numbers**](https://en.wikipedia.org/wiki/Ordered_Bell_number)

- Into non-crossing partitions **-> Catalan number**

- With block lengths given by the $k$th integer partition of the number of elements [**-> A036040**](https://oeis.org/A036040)

- Into blocks of equal size [**-> A038041**](https://oeis.org/A038041)

- Into blocks of different sizes [**-> A007837**](https://oeis.org/A007837)
- Such that the smallest block has size $k$ [**-> A182930**](https://oeis.org/A182930)

## Number of partitions into $k$  blocks
- ...and no restrictions [**(Stirling number of the second kind)**](stirlingNumbers.md)
 
  - ...and at least $k$ elements per block [**(associated Stirling number of the second kind)**](associatedStirling.md)
  - ...and at most $k$ elements per block [**(restricted Stirling  number of the second kind)**](restrictedStirling.md)
  - ...and the first $r$ elements are in separate blocks [**(r-Stirling number of the second kind)**](r-restrictedStirling.md)
  - ...and elements with pairwise distance $<d$ are in separate blocks [**(reduced Stirling number of the second kind)** ](reducedStirling.md)
- Such that the blocks aren't ordered but the elements in them are [**-> Lah numbers**](https://en.wikipedia.org/wiki/Lah_number)



## Parity Restrictions
[Peter Luschny: set partitions](https://oeis.org/wiki/User:Peter_Luschny/SetPartitions)
- Odd block size [**-> A003724**](https://oeis.org/A003724)
- Even block size [**-> A005046**](https://oeis.org/A005046)
- Odd number of blocks [**-> A024429**](https://oeis.org/A024429)
- Even number of blocks [**-> A024430**](https://oeis.org/A024430)
- Odd number of blocks, odd block size [**-> A003712**](https://oeis.org/A003712)
- Odd number of blocks, even block size [**-> A059385**](https://oeis.org/A059385)
- Even number of blocks, odd block size [**-> A003709**](https://oeis.org/A003709)
- Even number of blocks, even block size [**-> A059386**](https://oeis.org/A059386)




## Extra
- Number of blocks of size $n$
- Such that there are no blocks with a cardinality belonging to a given set set
# Resources
[1] https://oeis.org/wiki/User:Peter_Luschny/SetPartitions


______

Created on 10/05/2024

Last updated on 14/05/2024