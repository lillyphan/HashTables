# HashTables

## Challenge 1

In the case that the function x % n is used as a hash function, the use of a prime number would create a better hash function than that of a composite 
number. When the keys of a map are randomized, a composite number works adequately to give an even distribution in the map. However, when the keys are 
patterned, the indices collide as shown by the example below.

- 10 % 4 = 2
- 20 % 4 = 0
- 30 % 4 = 2
- 40 % 4 = 0

- 10 % 7 = 3
- 20 % 7 = 6
- 30 % 7 = 2
- 40 % 7 = 5

To avoid collisions, n must share as little common factors with the hash value as possible. To achieve this, n should be a number with feew factor, AKA,
a prime number.
