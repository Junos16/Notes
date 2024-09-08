# Algorithm
```
Quicksort(A,l,r):
	if l<r:
		q = Partition(A,l,r)
		Quicksort(A,l,q-1)
		Quicksort(A,q+1,r)
```

```
Partition(A,l,r):
	x = A[r]
	i = l-1
	for j = l to r-1:
		if A[j] <= x:
			i++
			swap(A[i], A[j])
	swap(A[i+1], A[r])
	return i+1
```
## Explanation
- Quicksort sorts the array using a divide and conquer approach
	- ***Divide:*** It divides the problem using another algorithm that partitions the array around a single element called the pivot $p$ such that there are two subarrays **LEFT$:=\{x:x\leq p\}$** and **RIGHT$:=\{x:x>p\}$**
	- ***Conquer:*** To conquer subproblems the Quicksort algorithm is called recursively on **LEFT** and **RIGHT** 
	- ***Combine:*** 
- Then the subarrays are sorted by calling Quicksort again
- 
# Partition (Deterministic)
## Proof of Correctness
## Time Complexity of Partition (Deterministic)
# Time Complexity of Quicksort (Deterministic)


