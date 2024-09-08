# Motivation for Hash Tables
- Data
## Direct Addressing
- If $|U|$ is very large then maintaining a table $T$ of size $|U|$ becomes impractical
	- There might not enough memory available on the system to hold a table of size $|U|$
	- The set of actual keys $K\subseteq U$ being stored might be much smaller than $U$ leading to a lot of wasted space
- Naively using the whole universe of keys leads to the 
## How to design a Hash Table
# Addressing Collisions

## Chaining
## Open Addressing

# Reducing Collisions
Choose a hash function that calculates the key in constant time and produces a uniform distribution of the keys from the universe
Using mod is a common strategy but use a prime number to prevent common factors leading to 
## Static Hashing
## Random Hashing

