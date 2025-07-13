
# 🧗 Hill Climbing Algorithm in C++

![Hill Climbing Banner](https://upload.wikimedia.org/wikipedia/commons/5/5a/Hill_Climbing.png)

> **Hill Climbing** is an iterative optimization algorithm that starts with an arbitrary solution and makes incremental changes to improve it. It moves to the neighbor with the best improvement, stopping at a local optimum.

---

## 📌 Features

* Simple, greedy optimization
* Moves to the best neighbor at each step
* Stops at local optimum (can use random restarts)
* Useful for function optimization and AI

---

## 🔧 How the Algorithm Works

Hill Climbing starts with an initial solution and iteratively moves to a better neighbor.

### 🧠 Key Concepts:
* `current`: Current solution/state
* `neighbor`: Possible next solutions

### 🔁 Process:
1. Start with an initial solution
2. Evaluate all neighbors
3. Move to the neighbor with the best improvement
4. Repeat until no neighbor is better (local optimum)

---

## 🛠 Sample Input/Output

### ✅ Input:
*(Depends on the specific problem; typically a starting state and a function to optimize)*

### 🕽 Output:
*(Sequence of states leading to a local optimum)*

---

## 🚀 Applications of Hill Climbing

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Optimization**     | Function and parameter optimization      |
| **Puzzles**          | N-Queens, Sudoku, etc.                   |
| **Machine Learning** | Feature selection, hyperparameter tuning |
| **Pathfinding**      | Finding optimal or near-optimal paths    |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(iterations * neighbors)` (problem dependent)    |
| **Space**        | `O(1)`                                             |

---

## 📄 Code Structure

* `main()` – Handles input and search loop
* `current`, `neighbor` – Represent states/solutions

---

## ✅ Dependencies

* C++ STL: `iostream`, `vector`

---

## 🧪 Try It Yourself

1. Compile using:
   ```bash
   g++ hill_climb.cpp -o hill_climb
   ./hill_climb
   ```
2. Input your problem and see the optimization in action!
