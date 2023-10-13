# Disjoint_set_maze
The aim is to randomly generate a maze and describe the maze as a set of cells and a set of walls. Using the disjoint-set data structure to compute the random maze. and testing it with a depth-first algorithm.

![](https://github.com/FrancescoZanella/Disjoint_set_maze/blob/main/maze.png)

## Implementation
The goal is to use the disjoint set data structure to generate a random maze with a real path that goes from the start s to end p. The step to implement it are:
  - Create the matrix of disjoint sets representing the walls, where each disjoint set is coupled with a cell
  - incrementally remove all the walls until the first set (starting point) and the last set (end point) are in the same set and so there is a path.
  - visualize the maze

## Profiling
Google benchmark has been used to evaluate the complexity of the algorithm. My implementation exhibits computational complexity as indicated in the benchmark below:
  - worst case: O(n^3)
  - average case: O(n^2)
  - best case: slightly more than O(1)

## How to Run the Code

1. Open the provided cpp code in a compatible environment (e.g. Google Colab).

2. Run the code step by step, following the order described in the code.

3. Under the secction Ouput you can specify the dimension of the maze:
  ```
  !./a.out rows cols
```
where you have to substitute rows and cols with your values.

## Example of output


![](https://github.com/FrancescoZanella/Disjoint_set_maze/blob/main/out.png)

**Description: example of output with 10 rows and 10 columns**

## Conclusion

This code is designed to address the data-structure challenge for mid course evalution for the Advanced Algorithms and Parallel Programming course at Polimi.
With this implementation  I have received 3 out of 2.

