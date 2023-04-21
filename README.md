# Theft detection visualization
# Introduction
Theft has always been a serious worry in society, resulting in enormous property loss
and a sense of insecurity. To address this issue, numerous measures have been
implemented, including the hiring of security professionals, the installation of
surveillance cameras, and the installation of alarms. These measures, however, have
limits and might sometimes fail to prevent theft.
To address this issue, we have developed a theft detection system using various
algorithms such as Breadth-First Search (BFS), Depth-First Search (DFS), and
Dijkstra's Algorithm. These algorithms have been widely used in the field of
computer-sciences and have proven to be effective in solving many real-world
problems.
Our system aims to detect theft by analyzing the movements of an object or person in a
given area. The algorithms used in this project will help us detect any suspicious
behavior or movement and alert us in real-time, thus preventing theft. In this project,
we've imagined the perpetrator as a spot or a dot in the matrix and any valuable object
prone to theft as another dot in the matrix. The burglars path to the object that must be
protected can be predicted based on the obstacles present in the path using multiple
algorithms ( bfs,dijkstra, and a* etc). We observe and contrast his actions with those of
other algorithms to determine which algorithm gives us the best outcome
# Prequisites:
1.You can run the python codes in any ide but we recommend to do so in Visual studio code. 
#
2.Create a virtual environment to enable the proper functioning of the libraries.
# Algorithm Working and implementation:
# BFS approach:
The proposed visualization project will utilize the Pygame library. The primary objective
is to generate a grid with randomly placed obstacles throughout the path. The program
will prompt the user to specify the number of rows and columns desired. To accomplish
this, we will import the random number generator and the deque option.
After defining the grid with random values, with a probability of less than twenty percent
for obstacle placement, the grid will be created in the required size. A function will be
written to draw those elements in the array with a value of 1 as obstacles. Another
function will be developed to determine neighboring cells to ensure that they do not
exceed the screen border and are not obstacles.
To find the path, we will apply the general breadth-first search (BFS) algorithm. The BFS
algorithm will construct the path from the origin (i.e., the top corner cell) to the cell
specified by the user. We will also write another function, known as get_click_mouse, to
adjust the position of the final path based on the user's preferences (i.e., valuable
object).
By using the BFS algorithm and visualization, we can observe how the perpetrator
reaches the goal state.
# Djikstra Approach:
A graph can be created to protect an area from theft. Each vertex represents a location,
and each edge represents a connection between two locations. Weights are assigned to
each edge based on the distance between locations, with high-security areas assigned
a higher weight.
A priority queue tracks the vertices to be processed, initialized with the starting vertex. A
dictionary tracks the distances from the starting vertex to each other vertex, initialized to
infinity except the starting vertex. Another dictionary tracks the previous vertex in the
shortest path to each vertex.
Dijkstra's algorithm is implemented to find the shortest path from the starting vertex to
all other vertices in the graph. At each iteration, the vertex with the lowest distance from
the priority queue is extracted, and the distances and previous vertices of its neighbors
are updated if a shorter path is found.
Once the algorithm has finished, the previous vertex dictionary is used to trace the
shortest path from each vertex to the starting vertex. If the shortest path from a vertex
to the starting vertex passes through the vertex representing the valuable object, that
vertex is marked as a potential theft location.
Testing and Refining: Test the algorithm using various scenarios, such as different
starting locations and high-security areas, to ensure its accuracy and efficiency. Once
the algorithm is working correctly, integrate it with a security system to automatically
detect and alert the personnel about potential theft locations.
Result and its visualization: Visualize the graph and the shortest paths using
PyCharm's built-in visualization tools. Highlight the potential theft locations in red, and
add labels or tooltips to indicate the shortest path to the security personnel location.
# A* approach:
Objective is to find the burglars path to the destination object using a* algorithm. The
path available is represented using a grid including obstacles and multiple ways to
reach the object. We will analyze the problem and application in practice of the main
algorithms for finding the shortest paths and not just the shortest but the most efficient
in terms of travel costs .
A* algorithm and its implementation: To implement the algorithm with a star we must
choose the appropriate heuristic function that will tell us how close we are to the
goal.
The A* algorithm uses a heuristic function to estimate the cost of the remaining path to
the destination from the current node. The algorithm works by exploring the nodes in the
grid, starting from the starting node and expanding to neighboring nodes based on their
estimated costs.
At each step, the algorithm selects the node with the lowest estimated cost and
continues the search until the destination is reached.
Testing and refining: After implementing the A* algorithm, we test it on different
scenarios to ensure it's working correctly. We can refine the algorithm by tweaking the
heuristic function or the way it selects nodes to optimize the pathfinding process.
