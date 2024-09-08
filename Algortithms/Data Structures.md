# Array Based Data Structures
- Unlike in mathematics where talking about sets is very common and convenient, in computer science arrays are the most fundamental data structure discussed
- Every other data structure is then implemented as a structure built using arrays
	- ***Example:*** A Graph is implemented as an adjacency matrix which is built using arrays or as an adjacency list that is also a list of arrays
- Arrays mirror the structure of memory in computers which makes them more fundamental to computer science as compared to data structures like sets, functions etc.
## Arrays
- Arrays are an ordered sequence of data
## Matrix
- An array of arrays can be used to represent a matrix
- ***Row Major Order:*** 
- ***Column Major Order*:**
## Stack
- 
## Queue
## Linked List
# Binary Heaps
## Binary Heaps
```
Heap(A,n):
	heap = A[n]
	size = n
	
	parent(i):
		return floor(i/2)
	left(i):
		return 2i
	right(i):
		return 2i+1
```

```	
max_heapify(A,i):
	l = A.left(i)
	r = A.right(i)
	if l<=A.size and A[l]>A[i]:
		largest = l
	else largest = i
	if r <= A.size and A[r]>A[largest]:
		largest = r
	if largest != i:
		temp = A[i]
		A[i] = A[largest]
		A[largest] = temp
		max_heapify(largest)
```

```
build_max_heap():
	
```
## Priority Queue
# Hash Tables
# Binary Search Trees
# Red and Black Trees
# Augmenting Data Structures
# B-Trees
# Data Structures for Disjoint Sets
