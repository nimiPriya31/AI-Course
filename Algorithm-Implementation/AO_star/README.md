
# 🌳 AO* (And-Or Star) Algorithm in C++

![AO* Banner](https://upload.wikimedia.org/wikipedia/commons/7/7e/And-or-graph.png)

> **AO*** is a search algorithm for AND-OR graphs, extending A* to problems where nodes can have AND/OR relationships. It is used in planning, reasoning, and game trees with complex dependencies.

---

## 📌 Features

* Solves AND-OR graph problems
* Interactive CLI for graph and heuristic input
* Shows step-by-step node selection and progress
* Demonstrates local minima (peaks) in search

---

## 🔧 How the Algorithm Works

AO* selects the most promising node based on heuristic values and expands it. If no neighbor has a better heuristic, it stops (local optimum).

### 🧠 Key Concepts:
* `heuristic[]`: Estimated cost from each node to goal
* `graph`: Adjacency list for AND-OR structure

### 🔁 Process:
1. Start at the initial node
2. At each step, move to the neighbor with the lowest heuristic
3. Stop when no neighbor improves the heuristic (peak)

---

## 🛠 Sample Input/Output

### ✅ Input:
```
Enter number of nodes: 4
Enter heuristic values:
3 2 1 0
Enter number of edges: 4
Enter edges (u v):
0 1
0 2
1 3
2 3
Enter start node: 0
```

### 🕽 Output:
```
Current: 0 with h=3
Current: 2 with h=1
Current: 3 with h=0
Reached peak at node: 3
```

---

## 🚀 Applications of AO* Algorithm

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **AI Planning**      | Automated planning and scheduling        |
| **Expert Systems**   | Reasoning with AND/OR dependencies      |
| **Game Trees**       | Solving games with AND/OR nodes         |
| **Problem Solving**  | Complex search in knowledge graphs      |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time (Worst)** | Exponential (depends on AND-OR graph structure)   |
| **Space**        | `O(n)` (number of nodes for graph and heuristics)  |

---

## 📄 Code Structure

* `main()` – Handles user input and search loop
* `heuristic[]` – Stores heuristic values
* `graph` – Adjacency list for AND-OR graph

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `limits`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ ao_star.cpp -o ao_star
   ./ao_star
   ```
2. Input your graph and heuristics to see the search in action!
