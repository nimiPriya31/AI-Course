# A* Search Algorithm

## How the Algorithm Works
A* (A-star) is a best-first search algorithm that finds the shortest path from a start node to a goal node in a weighted graph. It uses both the actual cost from the start and a heuristic estimate to the goal, combining them as `f(n) = g(n) + h(n)`, where:
- `g(n)`: Cost from the start node to node `n`.
- `h(n)`: Heuristic estimate from node `n` to the goal.
The algorithm explores nodes with the lowest `f(n)` value first, ensuring optimal and efficient pathfinding when the heuristic is admissible.

## Applications
- Pathfinding in maps and games (e.g., navigation for characters)
- Robot motion planning
- Network routing
- Puzzle solving (e.g., sliding puzzles, Rubik's cube)

## Complexity
- **Time Complexity:** O(E), where E is the number of edges (worst case, similar to Dijkstra's if heuristic is zero)
- **Space Complexity:** O(V), where V is the number of vertices (for storing open/closed sets)

## Sample Input & Output
**Input:**
```
Enter number of nodes: 4
Enter heuristic values for each node:
Node 1: 0 7
Node 2: 1 6
Node 3: 2 2
Node 4: 3 0
Enter number of edges: 4
Is the graph undirected? (1 for Yes, 0 for No): 1
Enter edges with cost (format: from to cost):
0 1 1
0 2 4
1 3 2
2 3 5
Enter start node: 0
Enter goal node: 3
```
**Output:**
```
A* Path from 0 to 3: 0 1 3
```
