---
title: Route-finding Algorithms
---


There are many ways to implement route-finding algorithms.
## Primitive Methods:

1. **Random backstepping** - Take one step at a time in the direction of the goal. If an obstacle is encountered try to work around it by backstepping a bit in a random direction and then trying again. Not reliable at all and will get stuck in a multitude of situations.

2. **Obstacle tracing** - Other approach, similar to random backstepping but instead of moving back randomly, start tracing around the object once a collision is found, as if you had the right hand stuck to the wall and had to move touching it. Once there's no collision continue moving in the goal's direction. Once again can get stuck in many situations.


## Methods that look ahead to find the entire path at once:
1. **Breadth First Search** - Simple graph traversal by visiting each layer of children at a time, stop when path is found. If the graph is unweighted (i.e. the distance between each adjacent node is always the same) it finds the shortest path although not too efficiently. For weighted graphs it might not return the shortest path, but will always find one if it exists.

2. **Depth First Search** - Another way to traverse a graph, but instead of taking it layer by layer, the algorithm tries to search deep into the graph first. This method can have problems if the depth of the search is not limited, especially when using a recursive implementation, which may lead to a stack overflow, so it is usually safer to implement it iteratively using a stack.

3. **Best First Search** - Similar to Breadth First Search but uses an heuristic that chooses the most promising neighbor first. The path returned may not be the shortest, but it's faster to run than breadth first search. A* is a type of Best First Search.

3. **Dijkstra's Method** - Keeps track of the total cost from the start to every node that is visited, and uses it to determine the best order to traverse the graph. Works with weighted graphs and returns the shortest path, but might involve a lot of searching.

4. **A**\*- Similar to Dijkstra but also uses an heuristic to estimate how likely each node is close to the goal, in order to make the best decision. Because of this heuristic, A* finds the shortest path in a weighted graph in a much more timely manner.
Then there are variations of A* (or pathfinding optimizations in general) that make it faster or more adapted to certain circunstances, such as (see related answer):

5. **D**\* (Dynamic) - Dynamic in the sense that it works under the assumption that the terrain can change even while you're still looking for the path.

7. **HPA**\* (Hierarchical) - Uses several layers at different abstraction levels to speed up the search. For instance, an higher level layer may simply connect rooms, while a lower level layer takes care of avoiding obstacles.

8. **IDA**\* (Iterative Deepening) - Reduces memory usage in comparison with regular A* by using iterative deepening.
SMA* (Simplified Memory-Bounded) - Only makes use of available memory to carry out the search.

9. **Jump Point Search** - Speeds up pathfinding on uniform-cost grid maps (link).