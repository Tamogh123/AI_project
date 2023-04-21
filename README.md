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
# Algorithm Working:
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
# Djikstra Approach
