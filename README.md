# Astar-Algorithm
<b>What is an A* Algorithm?</b><p>
It is a search algorithm used to find the shortest path between an initial and a final point. It is often used for map traversal to find the shortest path. A* was initially designed as a graph traversal problem to help build a robot that can find its own course. It remains a widely popular algorithm for graph traversal. It searches for shorter paths first, thus making it an optimal and complete algorithm. An optimal algorithm will find the least cost outcome for a problem, while a complete algorithm finds all the possible outcomes of a problem.

<b>Why A* Search Algorithm?</b><p>
A* Search Algorithm is a simple and efficient search algorithm that can be used to find the optimal path between two nodes in a graph. It will be used for the shortest path finding. It is an extension of Dijkstra’s shortest path algorithm (Dijkstra’s Algorithm). The extension here is that, instead of using a priority queue to store all the elements, we use heaps (binary trees) to store them. The A* Search Algorithm also uses a heuristic function that provides additional information regarding how far away from the goal node we are. This function is used in conjunction with the f-heap data structure in order to make searching more efficient.

<b>The Basic Concept of A* Algorithm</b><p>
A heuristic algorithm sacrifices optimality, with precision and accuracy for speed, to solve problems faster and more efficiently. All graphs have different nodes or points which the algorithm has to take, to reach the final node. The paths between these nodes all have a numerical value, which is considered as the weight of the path. The total of all paths transverse gives you the cost of that route.

Initially, the Algorithm calculates the cost to all its immediate neighboring nodes,n, and chooses the one incurring the least cost. This process repeats until no new nodes can be chosen and all paths have been traversed. Then, you should consider the best path among them. If f(n) represents the final cost, then it can be denoted as :

<b><i>f(n) = g(n) + h(n), where :

g(n) = cost of traversing from one node to another. This will vary from node to node

h(n) = heuristic approximation of the node's value. This is not a real value but an approximation cost</b></i>

<b>Explanation</b><p>
In an event when we have a grid with many obstacles and we want to get somewhere as rapidly as possible, the A* Search Algorithms are our savior. From a given starting cell, we can get to the target cell as quickly as possible. It is the sum of two variables’ values that determines the node it picks at any point in time. 

<img src="../main/Image/image.png" alt="Grid"></img>

At each step, it picks the node with the smallest value of ‘f’ (the sum of ‘g’ and ‘h’) and processes that node/cell. ‘g’ and ‘h’ is defined as simply as possible below:
<ul>
<li>‘g’ is the distance it takes to get to a certain square on the grid from the starting point, following the path we generated to get there.</li> 
<li>‘h’ is the heuristic, which is the estimation of the distance it takes to get to the finish line from that square on the grid.</li></ul>

Heuristics are basically educated guesses. It is crucial to understand that we do not know the distance to the finish point until we find the route since there are so many things that might get in the way.