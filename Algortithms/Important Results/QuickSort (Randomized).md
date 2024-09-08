# Algorithm
```
Randomized_Quicksort(A,l,r):
	if l<r:
		q = Randomized_Partition(A,l,r)
		Randomized_Quicksort(A,l,q-1)
		Randomized_Quicksort(A,q+1,r)
```

```
	Randomized_Partition(A,l,r):
	i = random(l,r)
	swap(A[r], A[i])
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
# 
