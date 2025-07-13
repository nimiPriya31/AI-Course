
# 🌐 Breadth-First Search (BFS) Algorithm in Python

![BFS Banner](https://upload.wikimedia.org/wikipedia/commons/4/46/Animated_BFS.gif)

> **Breadth-First Search (BFS)** is a classic graph traversal algorithm that explores all neighbors at the current depth before moving to the next level. It is widely used for shortest path finding, connectivity, and more.

---

## 📌 Features

* Level-order traversal of graphs
* Uses a queue for node management
* Finds shortest path in unweighted graphs
* Simple and efficient implementation

---

## 🔧 How the Algorithm Works

BFS starts at a source node and explores all its neighbors before moving to the next level.

### 🧠 Key Concepts:
* `queue`: Stores nodes to visit next
* `visited`: Tracks visited nodes

### 🔁 Process:
1. Add the start node to the queue and mark as visited
2. While the queue is not empty:
   * Remove the front node and process it
   * Add all unvisited neighbors to the queue
3. Repeat until all reachable nodes are visited

---

## 🛠 Sample Input/Output

### ✅ Input:
*(No user input; the graph is hardcoded in the code)*

### 🕽 Output:
```
A B C D E F G H I
```
*(BFS traversal starting from node 'A')*

---

## 🚀 Applications of BFS

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Pathfinding**      | Shortest path in unweighted graphs       |
| **Web Crawling**     | Exploring web links                      |
| **Social Networks**  | Finding degrees of separation            |
| **Network Routing**  | Broadcast and multicast routing          |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(V + E)` (V = vertices, E = edges)               |
| **Space**        | `O(V)`                                             |

---

## 📄 Code Structure

* `main()` – Calls the BFS function
* `bfs()` – Core logic for BFS traversal
* `graph` – Dictionary representing the graph

---

## ✅ Dependencies

* Python: `collections.deque`

---

## 🧪 Try It Yourself

1. Run using:
   ```bash
   python bfs.py
   ```
2. Observe the BFS traversal output!
