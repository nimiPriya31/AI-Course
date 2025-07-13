
# 🌲 Depth-First Search (DFS) Algorithm in Python

![DFS Banner](https://upload.wikimedia.org/wikipedia/commons/7/7f/Depth-First-Search.gif)

> **Depth-First Search (DFS)** is a fundamental graph traversal algorithm that explores as far as possible along each branch before backtracking. It is widely used for pathfinding, cycle detection, and more.

---

## 📌 Features

* Explores graph deeply before backtracking
* Uses stack (explicit or recursion)
* Finds paths, detects cycles, and more
* Simple and efficient implementation

---

## 🔧 How the Algorithm Works

DFS starts at a source node and explores as far as possible along each branch before backtracking.

### 🧠 Key Concepts:
* `stack`: Stores nodes to visit next (explicit or via recursion)
* `visited`: Tracks visited nodes

### 🔁 Process:
1. Add the start node to the stack and mark as visited
2. While the stack is not empty:
   * Pop the top node and process it
   * Add all unvisited neighbors to the stack
3. Repeat until all reachable nodes are visited

---

## 🛠 Sample Input/Output

### ✅ Input:
*(No user input; the graph is hardcoded in the code)*

### 🕽 Output:
```
A B G H I C D E F
```
*(DFS traversal starting from node 'A')*

---

## 🚀 Applications of DFS

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Pathfinding**      | Finding paths in mazes and puzzles       |
| **Cycle Detection**  | Detecting cycles in graphs               |
| **Topological Sort** | Ordering tasks with dependencies         |
| **Connected Comp.**  | Finding connected components             |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(V + E)` (V = vertices, E = edges)               |
| **Space**        | `O(V)`                                             |

---

## 📄 Code Structure

* `main()` – Calls the DFS function
* `dfs()` – Core logic for DFS traversal
* `graph` – Dictionary representing the graph

---

## ✅ Dependencies

* Python: No external dependencies

---

## 🧪 Try It Yourself

1. Run using:
   ```bash
   python dfs.py
   ```
2. Observe the DFS traversal output!
