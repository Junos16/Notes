# Generic Algorithms
```
GENERIC_MST(G,w)
	A = empty
	while A does not form a spanning tree
		find an edge (u,v) that is safe for A
		A = A union {(u,v)}
	return A
```
# Specific Algorithms
## Kruskal's Algorithm
```
MST_KRUSKAL(G,w)
	A = empty
	for each vertex in G.V
		MAKE_SET(v)
	create a single list of the edges in G.E
	sort the list  of edges into monotonically increasing order by weight w
	for each edge (u,v) taken from the sorted list in the order
		if FIND_SET(u) != FIND_SET(v)
			A = A union {(u,v)}
			UNION(u,v)
	return A
```
## Prim's Algorithm
```
MST_Prim(G,w,r)
	for each vertex u in G.V
		u.key = inf
		u.pi = NIL
	r.key = 0
	Q = empty
	for each u in G.V
		INSERT(Q,u)
	while Q != empty
		u = EXTRACT_MIN(Q)
		for each vertex v in G.Adj[u]
			if v in Q and w(u,v) < v.key
				v.pi = u
				v.key = w(u,v)
				DECREASE_KEY(Q,v,w(u,v))
				
```
