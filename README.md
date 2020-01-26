# ant-colony-tsp
Solve TSP using Ant Colony Optimization in Python 3

### Requirements
* Python3
* matplotlib

### Usage
Run `python main.py` to see the results.

### Inference 
![](https://github.com/10-zin/acotsp/blob/master/shortest_path_graphs/path_graphs.png)

The four optimal  paths above illustrate the shortest path found by ACO for the Travelling Salesman Problem. Here x and y axis are simply the coordinates of each point (blue dots) and the path is represented by the red line connecting the dots. The number of points shown in the graphs are 10, 50, 90 and 130 respectively from top left to bottom right.

![](https://github.com/10-zin/acotsp/blob/master/generational_graphs/gen-graphs.jpg)
The four paths above illustrate 4 generations needed for aco to find the optimal path for tsp of 30 points. Their costs are 17342.384, 16568.878, 16021.089 and 15736.696 respectively from top left to bottom right.

![](https://github.com/10-zin/acotsp/blob/master/misc_graphs/cost-time.jpg)
The two graphs above illustrate the cost of path(euclidean distance) and time(in seconds) to find optimal path as y axis with respect to the number of points as the x axis.
