
# 🏁 Best First Search Algorithm in C++

![Best First Search Banner](https://upload.wikimedia.org/wikipedia/commons/6/6a/Best-First-Search.gif)

> **Best First Search** is a greedy search algorithm that expands the most promising node chosen by a heuristic. It is used for fast pathfinding and problem-solving, though it may not always find the shortest path unless the heuristic is admissible.

---

## 📌 Features

* Greedy search using a priority queue
* Finds a path from source to target
* Demonstrates path output in C++
* Simple, clear code structure

---

## 🔧 How the Algorithm Works

Best First Search uses a priority queue to always expand the node with the lowest heuristic value.

### 🧠 Key Concepts:
* `heuristic[]`: Estimated cost for each node
* `priority queue`: Expands node with lowest heuristic

### 🔁 Process:
1. Start from the source node
2. Add to priority queue with heuristic value
3. Expand the node with the lowest heuristic
4. Mark as visited and add neighbors
5. Repeat until the target is found

---

## 🛠 Sample Input/Output

### ✅ Input:
*(No user input; the graph and edges are hardcoded in the code)*

### 🕽 Output:
```
0 1 4 9
```
*(Path from source 0 to target 9)*

---

## 🚀 Applications of Best First Search

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Pathfinding**      | AI and games, navigation                 |
| **Puzzle Solving**   | Solving mazes, puzzles                   |
| **Web Crawling**     | Efficiently traversing web links         |
| **Network Routing**  | Finding efficient network paths          |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(E log V)` (E = edges, V = vertices)             |
| **Space**        | `O(V)`                                             |

---

## 📄 Code Structure

* `main()` – Sets up the graph and calls the search
* `bestFirstSearch()` – Core logic for Best First Search
* `edgeList` – List of graph edges

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `queue`, `algorithm`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ best_first.cpp -o best_first
   ./best_first
   ```
2. Observe the path output from source to target!
