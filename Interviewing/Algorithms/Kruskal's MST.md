Pseudocode
``` 
1. Sort all edges in non-increasing order
2. For all edges in order
	a. if it doesn't form an edge int he spanning tree so far, add it to the spanning tree
3. Repeat 2 until there are V-1 edges
```

For finding cycle use [[Union-Find]] 