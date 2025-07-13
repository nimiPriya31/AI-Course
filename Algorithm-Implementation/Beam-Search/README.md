
# 🌬️ Beam Search Algorithm in C++

![Beam Search Banner](https://upload.wikimedia.org/wikipedia/commons/2/2c/Beam_search.png)

> **Beam Search** is a heuristic search algorithm that explores a graph by expanding only a limited set of the most promising nodes at each level, determined by a fixed beam width. It is widely used in AI, NLP, and robotics for efficient, memory-bounded search.

---

## 📌 Features

* User-defined beam width for memory control
* Interactive CLI for graph and heuristic input
* Finds goal node efficiently or reports failure
* Demonstrates level-wise node selection

---

## 🔧 How the Algorithm Works

Beam Search keeps only the best `k` nodes (beam width) at each level, discarding the rest. It uses a heuristic to rank nodes and expands the most promising ones.

### 🧠 Key Concepts:
* `beam width`: Number of nodes kept at each level
* `heuristic[]`: Estimated cost for each node

### 🔁 Process:
1. Start from the initial node
2. At each level, expand all current nodes
3. Rank all children by heuristic and keep the best `k`
4. Repeat until the goal is found or no nodes remain

---

## 🛠 Sample Input/Output

### ✅ Input:
```
Enter number of nodes and edges: 5 6
Enter heuristic values:
3 2 1 4 0
Enter edges (u v):
0 1
0 2
1 3
2 4
3 4
1 2
Enter start, goal, and beam width: 0 4 2
```

### 🕽 Output:
```
Goal found at node 4
```

---

## 🚀 Applications of Beam Search

| Application Area     | Use Case                                         |
| -------------------- | ------------------------------------------------ |
| **NLP**              | Machine translation, speech recognition          |
| **Robotics**         | Pathfinding with memory constraints              |
| **Sequence Models**  | Sequence prediction, text generation             |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(b * d * log b)` (b = beam width, d = depth)     |
| **Space**        | `O(b * d)`                                         |

---

## 📄 Code Structure

* `main()` – Handles user input and search loop
* `heuristic[]` – Stores heuristic values
* `graph` – Adjacency list for the graph

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `queue`, `algorithm`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ Beam.cpp -o beam_search
   ./beam_search
   ```
2. Input your graph, heuristics, and beam width to see the search in action!
