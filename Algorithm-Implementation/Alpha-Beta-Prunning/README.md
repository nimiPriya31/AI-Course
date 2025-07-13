
# ♟️ Alpha-Beta Pruning Algorithm in C++

![Alpha-Beta Pruning Banner](https://upload.wikimedia.org/wikipedia/commons/9/91/Alpha-beta_pruning.svg)

> **Alpha-Beta Pruning** is a powerful optimization for the Minimax algorithm, widely used in AI for two-player games. It prunes branches in the game tree that cannot affect the final decision, making search much faster without sacrificing optimality.

---

## 📌 Features

* Efficiently prunes unnecessary branches in game trees
* Returns the optimal value for the maximizer
* Demonstrates tree setup and evaluation in C++
* Clear output of the optimal value

---

## 🔧 How the Algorithm Works

Alpha-Beta Pruning traverses the game tree, maintaining two values:

* `alpha`: Best value that the maximizer can guarantee so far
* `beta`: Best value that the minimizer can guarantee so far

### 🔁 Process:
1. Traverse the tree using Minimax logic
2. At each node, update `alpha` and `beta`
3. If `beta <= alpha`, prune the branch (no need to explore further)
4. Continue until the optimal value is found

---

## 🛠 Sample Input/Output

### ✅ Input:
*(No user input; the tree and values are hardcoded in the code)*

### 🕽 Output:
```
Optimal value using Alpha-Beta Pruning: 6
```

---

## 🚀 Applications of Alpha-Beta Pruning

| Application Area     | Use Case                                      |
| -------------------- | --------------------------------------------- |
| **Game AI**          | Chess, Tic-Tac-Toe, Checkers, Connect Four    |
| **Decision Making**  | Adversarial search in two-player games        |
| **AI Agents**        | Any scenario using Minimax for best decisions |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                                      |
| ---------------- | --------------------------------------------------------------- |
| **Time (Worst)** | `O(b^d)` (b = branching factor, d = depth)                      |
| **Time (Best)**  | `O(b^{d/2})` with perfect ordering (much faster than Minimax)   |
| **Space**        | `O(bd)` (recursion stack and tree representation)               |

---

## 📄 Code Structure

* `main()` – Sets up the tree and calls the algorithm
* `alphaBeta()` – Core logic for Alpha-Beta Pruning
* `adjMatrix` – Adjacency matrix for tree structure
* `values[]` – Leaf node values

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`, `algorithm`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ alpha_beta_adj.cpp -o alpha_beta
   ./alpha_beta
   ```
2. Observe the output for the optimal value!
