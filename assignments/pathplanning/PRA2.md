# Implementation and comparison of heuristics for path-planning


## Objectives

* Compare Dijkstra, A* and Theta* algorithms.
* Implement Theta* and some heuristics.
* Understand the impact of the heuristic selection in path-planning.
* Use a graphical interface to visualize the results.

## Dependencies

Install [PathPlanPrinter](https://github.com/R012/PathPlanPrinter), which depends on the libraries numpy and PIL or Pillow. Read the README.md file in the project's root folder for instructions about the usage.

In order to make a local copy, please do the following:
1. Open a terminal a place where you want to locally copy the directory.
2. Clone the folder using the command:

 `git clone https://github.com/R012/PathPlanPrinter.git`

## Practical assignment

Perform the following tasks:

1. Use the the functions provide in the documentation to visualize paths on images. 

2. Consider that the robot is initially located at the position (18,19) and the goal is to be at position (12,12). Visualizes the computed path using the Dijkstra algorithm. Change the initial point to  (27,19) and the goal point to (8,20).
   
3. We provide you with the implementation of A* and Dijkstra. The implementation of A* is based on the  pseudo-code of the next figure:

<img align="center" src="A*.png" width="600">

4. Implement Theta* using the following pseudo-code:

<img align="center" src="Theta*.png" width="600">

Take into account that the difference between A* and Theta* is the Line of sight. Here is the code to calculate it:

<img align="center" src="Lineofsight.png" width="600">

5. Which heuristic is used by default? If needed, use the path-planning visualizer in https://qiao.github.io/PathFinding.js/visual/ to reconstruct the scenario and observe the node expansion using different algorithms.

6. Implement the Manhattan and Euclidean heuristics for A*/Theta*. Both functions take the initial and final points as tuples (X, Y) and must return a float with the heuristic value.

8. Run the 3 algorithms and compare the results, changing when appropriate the heuristic.