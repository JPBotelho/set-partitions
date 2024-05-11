# bloom-filters

# The Bloom Filter

### Main purpose
Testing whether an element belongs in a set.

### Main idea
Allow some false positives, save a lot of memory.

### Introduced in
Howard bloom's paper.

### Problems
False positives.

Not cache friendly.

Can't remove items.

### Real-world uses
https://redis.io/docs/latest/develop/data-types/probabilistic/bloom-filter/

### Extensions

There are many bloom-filter inspired data structures. Here are some of the motivations for them:

#### Frequency estimation

#### Removing Items

#### Improving Performance when all the possible sets are known beforehand