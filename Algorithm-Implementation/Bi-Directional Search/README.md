
# 🔄 Bi-Directional Search Algorithm in C++

![Bi-Directional Search Banner](https://upload.wikimedia.org/wikipedia/commons/5/5d/Bidirectional_search.gif)

> **Bi-Directional Search** runs two simultaneous searches—one forward from the start and one backward from the goal. The search stops when the two meet, greatly reducing the search space for shortest path problems.

---

## 📌 Features

* Simultaneous forward and backward search
* Efficient for shortest path in large graphs
* Interactive CLI for graph input
* Reports depth at which target is found

---

## 🔧 How the Algorithm Works

Bi-Directional Search alternates between expanding nodes from the start and goal until the searches meet.

### 🧠 Key Concepts:
* `queueStart`, `queueTarget`: Queues for forward and backward search
* `visitedStart`, `visitedTarget`: Visited sets for both directions

### 🔁 Process:
1. Start BFS from both start and goal nodes
2. Alternate expanding nodes from each direction
3. If a node is visited by both searches, path is found
4. Report the depth or failure

---

## 🛠 Sample Input/Output

### ✅ Input:
```
Enter the number of vertices: 6
Enter the number of edges: 7
Enter the edges (vertex1 vertex2):
0 1
0 2
1 3
2 4
3 4
3 5
4 5
Enter the starting vertex: 0
Enter the target vertex: 5
```

### 🕽 Output:
```
Target vertex found at depth 2
```

---

## 🚀 Applications of Bi-Directional Search

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Pathfinding**      | Shortest path in large graphs            |
| **Route Planning**   | GPS, maps, navigation systems            |
| **Puzzle Solving**   | Efficiently solving state-space puzzles  |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(b^{d/2})` (b = branching factor, d = distance)  |
| **Space**        | `O(b^{d/2})`                                       |

---

## 📄 Code Structure

* `main()` – Handles input and starts the search
* `bidirectionalSearch()` – Core logic for bi-directional search
* `graph` – Adjacency list for the graph

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `queue`, `unordered_set`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ bidirectional.cpp -o bidirectional
   ./bidirectional
   ```
2. Input your graph and see the search in action!
