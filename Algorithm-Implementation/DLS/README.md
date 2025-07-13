
# 🪜 Depth-Limited Search (DLS) Algorithm in C++

![DLS Banner](https://upload.wikimedia.org/wikipedia/commons/7/7f/Depth-First-Search.gif)

> **Depth-Limited Search (DLS)** is a DFS variant that limits the search to a specified depth, preventing infinite loops in cyclic or infinite graphs. It is useful for puzzles, games, and large graphs.

---

## 📌 Features

* DFS with a maximum depth limit
* Prevents infinite loops in deep or cyclic graphs
* Reports if the target is found within the limit
* Simple and efficient implementation

---

## 🔧 How the Algorithm Works

DLS performs DFS but stops recursion when the depth limit is reached.

### 🧠 Key Concepts:
* `maxDepth`: Maximum allowed search depth
* `visited[]`: Tracks visited nodes

### 🔁 Process:
1. Start DFS from the initial node at depth 0
2. At each recursive call, increment depth
3. If depth > maxDepth, stop recursion
4. If target is found, report success

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
0 1 3 4
Target found
```

---

## 🚀 Applications of DLS

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Puzzles**          | Solving with depth constraints           |
| **Game Trees**       | Exploring moves up to a certain depth    |
| **Large Graphs**     | Avoiding infinite loops                  |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(b^l)` (b = branching factor, l = depth limit)   |
| **Space**        | `O(l)` (recursion stack)

---

## 📄 Code Structure

* `main()` – Handles input and starts DLS
* `dfs()` – Core logic for depth-limited search
* `g[]` – Adjacency list for the graph

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `cstring`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ DLS.cpp -o dls
   ./dls
   ```
2. Input your graph and depth limit to see DLS in action!
