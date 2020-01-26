# ant-colony-tsp
Solving the Travelling Salesman Problem using Ant Colony Optimization.

### Dataset
TSP requires points and their coordinates to provide a basis of forming a possible path, hence, a dataset with 3 columns consisting of the label of point - x-coordinate and y-coordinate - is created. The following table illustrates the basic schema of this dataset.

| Point | X-Coordinate | Y-coordinate|
|-------|--------------|-------------|
|1      | 23           | 67          |
|2      |45            | 99          |

However, for robust evaluation of ACO in solving the TSP problem, a total of 7 dependent datasets of x points is created, where : ![](https://latex.codecogs.com/gif.latex?x%20%5Cin%20%5C%7B%2010n%20%3A%20n%5Cin%202k&plus;1%2C%20where%20%5C%20k%20%5Cin%20%5C%7B0%2C%202%2C%20..6%5C%7D%20%5C%7D).  They are created such that each dataset of n points has all similar points as the dataset with n- points, where  denotes the number of newly added points in the graph This structure helps in a better interpretation of the tests as it creates a fair prior for comparison. Moreover, dataset starts with 10 points and ends with a dataset of 130 points. 
The distance between two points are calculated using the standard euclidean distance formula for 2 dimensional space based on the end point coordinates. if p = (p1, p2) and q = (q1, q2) then the distance is given by: ![](https://latex.codecogs.com/gif.latex?d%28p%2C%20q%29%20%3D%20%5Csqrt%7B%28q_%7B1%7D-%20p_%7B1%7D%29%5E2%20&plus;%20%28q_%7B2%7D-%20p_%7B2%7D%29%5E2%7D)

### Usage
Run `pip install requirements.txt`

Run `python main.py` to see the results.

### Inference 
![](https://github.com/10-zin/acotsp/blob/master/shortest_path_graphs/path_graphs.png)

*The four optimal  paths above illustrate the shortest path found by ACO for the Travelling Salesman Problem. Here x and y axis are simply the coordinates of each point (blue dots) and the path is represented by the red line connecting the dots. The number of points shown in the graphs are 10, 50, 90 and 130 respectively from top left to bottom right.*

![](https://github.com/10-zin/acotsp/blob/master/generational_graphs/gen-graphs.jpg)
*The four paths above illustrate 4 generations needed for aco to find the optimal path for tsp of 30 points. Their costs are 17342.384, 16568.878, 16021.089 and 15736.696 respectively from top left to bottom right.*

![](https://github.com/10-zin/acotsp/blob/master/misc_graphs/cost-time.jpg)
*The two graphs above illustrate the cost of path(euclidean distance) and time(in seconds) to find optimal path as y axis with respect to the number of points as the x axis.*
