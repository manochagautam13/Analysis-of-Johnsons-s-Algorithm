# Analysis-of-Johnsons-s-Algorithm
Implemented different types of heaps (array,binary heap,binomial heap,fibonacci heap) to run the Dijkstra portion of the Johnson's Algorithm to analyze the time complexity for each one of them.

Input Format:
 First line: Number of Test Cases T and then follows their description For each test case, First line/row indicate N D (single space separated) where N is number of vertices in directed graph where vertices are labelled 1 to N (not 0 indexing) D specifies whether Directed Graph or undirected graph (D=0 means undirected, else it is directed) This is then followed by N lines each containing N integers (basically NxN Adjacency or say weight matrix representation of the graph of that test case). The NxN matrix values / integers denote the edge-weights, there are no self-loops in the graph, and the weight=999999 indicates that there is no edge between those two vertices considered. //Diagonal entries will always be zero and one can safely assume no edge from vertex to itself.
 
 Output Format:
  For each test case, there are as many rows as many number of vertices in that graph under consideration. Consider if the test case has N vertices, then N rows each containing N single space separated values s.t. the kth value in ith row tells the distance of kth vertex from the (source) vertex i. (Kind of NxN shortest path matrix) Print 999999 if the vertex is not reachable from the source vertex considered. Print just one value -1 in the row - if for that row, the shortest path is not well defined or say, there is reachable negative weight cycle. There must be also one last row at end of outputs for T testcases, where last row has T entries indicative of time taken for different test cases that were considered.
  
  Constraints: 0 ≤ T ≤ 2000 1 ≤ N ≤ 10 million -999 ≤ Adj matrix values ≤ 999
