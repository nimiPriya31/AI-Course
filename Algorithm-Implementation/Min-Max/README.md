
# 🎲 Min-Max Algorithm in Python

![Min-Max Banner](https://upload.wikimedia.org/wikipedia/commons/9/9b/Minimax_example.svg)

> **Min-Max** is a recursive algorithm used in decision-making and game theory. It finds the optimal move for a player, assuming the opponent also plays optimally. Widely used in AI for games like Chess and Tic-Tac-Toe.

---

## 📌 Features

* Recursive evaluation of game trees
* Handles both maximizer and minimizer turns
* Finds the best achievable score for the player
* Simple, clear implementation in Python

---

## 🔧 How the Algorithm Works

Min-Max explores all possible moves, recursively evaluating the minimum and maximum values at each level until reaching terminal states (leaf nodes).

### 🧠 Key Concepts:
* `maxTurn`: Boolean indicating maximizer or minimizer
* `score[]`: List of leaf node values

### 🔁 Process:
1. Start at the root node
2. Recursively evaluate left and right children
3. At maximizer's turn, pick the maximum value
4. At minimizer's turn, pick the minimum value
5. Continue until reaching leaf nodes

---

## 🛠 Sample Input/Output

### ✅ Input:
```
Enter the number of leaf node: 4
Enter the score of leaf node1: 3
Enter the score of leaf node2: 5
Enter the score of leaf node3: 2
Enter the score of leaf node4: 9
```

### 🕽 Output:
```
The score of the leaf node is: The best score is: 5
```

---

## 🚀 Applications of Min-Max

| Application Area     | Use Case                                 |
| -------------------- | ---------------------------------------- |
| **Game AI**          | Chess, Tic-Tac-Toe, Checkers             |
| **Decision Making**  | Adversarial environments                 |

---

## ⏱ Time & Space Complexity

| Metric           | Complexity                                         |
| ---------------- | -------------------------------------------------- |
| **Time**         | `O(b^d)` (b = branching factor, d = tree depth)    |
| **Space**        | `O(bd)`                                            |

---

## 📄 Code Structure

* `main()` – Handles input and calls minmax
* `minmax()` – Core logic for Min-Max recursion
* `score[]` – List of leaf node values

---

## ✅ Dependencies

* Python: `math`

---

## 🧪 Try It Yourself

1. Run using:
   ```bash
   python minmax.py
   ```
2. Input your leaf node scores and see the best score!
