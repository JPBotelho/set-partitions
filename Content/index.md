<!-- title: Set Partitions -->

# Set partitions

In this website are resources on counting set partitions and related structures.

It is not a complete reference. These are just some of the things I learned about when studying this topic. I made this website because it would've been of great help to me. 

There might be mistakes, double check with the given sources when in doubt.

 If there is something you feel should be added, removed or changed, contact me at jpbotelho.costa (at) gmail.com

## Named restrictions

### Bell numbers

- [**Bell Number**](bellNumbers.md) - with no restrictions 

- [**Associated Bell number**](associatedBell.md) - $\geq m$ elements per block
  
- [**Restricted Bell number**](restrictedBell.md) - $\leq m$ elements per block


- [**r-Bell number**](r-bell.md) - the first $r$ elements are in separate blocks 

- [**Restricted r-Bell number**](#) - the first $r$ elements are in separate blocks, $\leq m$ elements per block

- [**Associated r-Bell number**](#) - the first $r$ elements are in separate blocks, $\geq m$ elements per block
  

- [**Reduced Bell number** ](reducedBell.md) - elements with pairwise distance $<d$ are in separate blocks 

### Stirling numbers
All of these are assumed to be Stirling numbers of the second king, ommitted to keep the titles short.

- [**Stirling number of the second kind**](stirlingNumbers.md) - $k$ blocks
 
- [**Associated Stirling number**](associatedStirling.md) - $k$ blocks and $\geq m$ elements per block
- [**Restricted Stirling number**](restrictedStirling.md) - $k$ blocks and $\leq m$ elements per block
- [**r-Stirling number**](r-restrictedStirling.md) - $k$ blocks, the first $r$ elements are in separate blocks
- [**Associated r-Stirling number**](#) - $k$ blocks, the first $r$ elements are in separate blocks, $\geq m$ elements per block
- [**Restricted r-Stirling number**]() - $k$ blocks, the first $r$ elements are in separate blocks, $\leq m$ elements per block
- [**Reduced Stirling number** ](reducedStirling.md) - $k$ blocks,elements with pairwise distance $< d$ are in separate blocks 

## Other restrictions

- [**$\geq m$ elements per block, and the largest block has $j$ elements**](https://math.stackexchange.com/questions/1078391/counting-set-partitions-with-constraints)

- [**Into blocks of equal size**](equalBlockSizes.md)

- [**Into blocks of distinct sizes**](distinctBlockSizes.md)
## Restriction on specific elements 

- [**Non-crossing partitions**](#)
- [**Non-nesting partitions**](#)




- Such that the blocks are ordered but the elements in them aren't [**-> ordered Bell / Fubini numbers**](https://en.wikipedia.org/wiki/Ordered_Bell_number)

- Into non-crossing partitions **-> Catalan number**

- With block lengths given by the $k$th integer partition of the number of elements [**-> A036040**](https://oeis.org/A036040)


- Such that the smallest block has size $k$ [**-> A182930**](https://oeis.org/A182930)



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