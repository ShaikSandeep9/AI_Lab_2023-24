DATE: 17/02/2024
REGISTER NUMBER : 212221060103
AIM:
To write a python program to implement Depth first Search.

Algorithm:
Start the program
Create the graph by using adjacency list representation
Define a function dfs and take the set “visited” is empty
Search start with initial node. Check the node is not visited then print the node.
For each neighbor node, recursively invoke the dfs search.
Call the dfs function by passing arguments visited, graph and starting node.
Stop the program.
Program:
graph = { '5' : ['3','7'], '3' : ['2', '4'], '7' : ['8'], '2' : [], '4' : ['8'], '8' : [] } visited = set() # Set to keep track of visited nodes of graph. def dfs(visited, graph, node): #function for dfs if node not in visited: print (node) visited.add(node) for neighbour in graph[node]: dfs(visited, graph, neighbour)

Driver Code
print("Following is the Depth-First Search") dfs(visited, graph, '5')

Output:Screenshot (17)
Result:
Thus the depth first search order was found sucessfully.

