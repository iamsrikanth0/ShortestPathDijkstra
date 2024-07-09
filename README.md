# ShortestPathDijkstra
Weight Graph
Concept is very simple- relaxtion.Source,...., u and V. if (dist[u]+wt < dist[v]) then dist[v]= dist[u]+wt
At each step we will have to find the Shortest path (like greedy), so we will have to use BFS to tranverse. 
At each step, we want a Node which is not yet visited and has a Short distance, how to get this data, we use priority Queue(dst based), so we will get the lowest distance neighbour.
Now once we get a Node, we will try to get the neighbours, but before directly getting from prioty Q, we perform relaxation, to see if there is any other short distance. 
So major concepts, PQ(for getting immediate short neighbours), Relaxation(alernate route for shortest path)
We do this till we tranverse all the neighbours, this can be tracked using Visted Array. Don't forget, we use Vis array primarily because grpahs has cycles. 
Try dry run to get clear picture. 
Intialization= create a PQ baseed on dst, dst array (include starting point distance), visited array
Pro tip: Whenever we need two values to validat everytim, create a Class for it. Here Node and Wt is needed everytime, so we shall create one.
