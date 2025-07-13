
# 🔁 Iterative Deepening Search (IDS) Algorithm in C++

![IDS Banner](https://upload.wikimedia.org/wikipedia/commons/7/7f/Depth-First-Search.gif)

> **Iterative Deepening Search (IDS)** combines the space efficiency of DFS with the optimality of BFS. It repeatedly applies Depth-Limited Search (DLS) with increasing depth limits until the goal is found or a maximum depth is reached.

---

## 📌 Features

* Combines DFS and BFS advantages
* Finds shallowest solution with low memory
* Interactive CLI for graph input
* Reports depth at which target is found

---

## 🔧 How the Algorithm Works

IDS performs DLS repeatedly, increasing the depth limit each time.

### 🧠 Key Concepts:
* `maxDepth`: Maximum allowed search depth
* `iddfs()`, `dfs()`: Iterative and recursive search functions

### 🔁 Process:
1. For depth = 0 to maxDepth:
   * Run DLS with current depth limit
   * If target is found, stop
2. If not found, report failure

---

## 🛠 Sample Input/Output

### ✅ Input:
```
5 4
0 1
0 2
1 3
1 4
0 4 2
```

### 🕽 Output:
```
Depth 0: 0
Depth 1: 0 1 2
Depth 2: 0 1 3 4
Target found at depth 2
```

---

## 🚀 Applications of IDS

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Pathfinding**      | Large graphs, shallowest solution        |
| **Game Trees**       | Exploring moves with memory efficiency   |
| **AI Planning**      | Planning with unknown solution depth     |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(b^d)` (b = branching factor, d = solution depth)|
| **Space**        | `O(d)` (recursion stack)

---

## 📄 Code Structure

* `main()` – Handles input and starts IDS
* `iddfs()`, `dfs()` – Core logic for iterative and depth-limited search
* `g[]` – Adjacency list for the graph

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `cstring`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ IDS.cpp -o ids
   ./ids
   ```
2. Input your graph and max depth to see IDS in action!
