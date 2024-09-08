# Algorithm
```
BFS(G,source)
	for each vertex u in G.V - {source}
		u.color = WHITE
		u.d = inf
		u.pi = NIL
	source.color = GRAY
	soure.d = 0
	source.pi = NIL
	Q = empty queue
	ENQUEUE(Q,source)
	while Q is not empty
		u = DEQUEUE(Q)
		for each vertex v in G.Adj[u]
			if v.color == WHITE
				v.color = GRAY
				v.d = u.d + 1
				v.pi = u
				ENQUEUE(Q,v)
		u.color = BLACK
```
## Explanation
- ***Aim:*** To try and traverse every vertex in the graph that is reachable from the source 
	- To try and maintain the depth at which each reachable vertex lies from the source
	- To maintain a tree where each branch shows the shortest path to travel to each vertex reachable from the source
- ***Explanation:*** 

# Analysis
## Time Complexity
## Correctness
- ***Shortest-Path Distance:*** $\delta(s,v)$ is the minimum number of edges in any path from vertex $s$ to $v$
	- ***Lemma:*** Let $G=(V,E)$ be a graph $\forall s\in V,(u,v)\in E\space \delta(s,v)\leq\delta(s,u)+1$ 
		- ***Proof:*** 
			- If either of $u$ or $v$ are unreachable from $s$ then so is the other $\implies\delta(s,v)=\delta(s,u)=\infty$, thus proving the statement
			- 
### Breadth-First Trees
