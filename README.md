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

To avoid collisions, n must share as little common factors with the hash value as possible. To achieve this, n should be a number with few factor, AKA,
a prime number.

## Challenge 2

Whether or not x % 599 would be a good hash function depends largely on the type of string being passed in. The string can vary from lowercase letters, uppercase letters, long, or short. In the scenario that the summation of characters is any less than 599 and are patterned, the distribution of values is not very even. For example, short (3 characters) strings made up of uppercase letters can have summation values ranged between 195 to 270. In this case, the indices of values would be very close to eachother and therefore not very well distributed. However, if the summation is larger than 599 (which can be achieved with longer strings or lowercase letters), the function will map out more evenly-distributed values.
