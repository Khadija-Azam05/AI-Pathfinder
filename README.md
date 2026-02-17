# 🧭 AIPathfinder
### Uninformed Search Algorithm Visualization

AIPathfinder implements and visualizes multiple **uninformed (blind) search algorithms** on a 10×10 grid environment.

The goal is to demonstrate how different search strategies explore the grid to find a path from the **Start node (S)** to the **Target node (T)** while avoiding obstacles.

The visualization displays:
- Frontier nodes
- Explored nodes
- Final reconstructed path

---

## 🚀 Features

- 10×10 grid environment  
- Static vertical wall obstacle  
- Step-by-step visualization using `matplotlib`  
- Menu-driven algorithm selection  
- Parent tracking for path reconstruction  
- Six uninformed search algorithms implemented  

---

## 🧠 Algorithms Implemented

### 1. Breadth-First Search (BFS)
- Uses a Queue (FIFO)
- Guarantees shortest path in an unweighted grid
- Explores level by level

### 2. Depth-First Search (DFS)
- Uses a Stack (LIFO)
- Goes deep before backtracking
- Does not guarantee shortest path

### 3. Uniform Cost Search (UCS)
- Uses a Priority Queue
- Expands lowest-cost node first
- Optimal for uniform step cost

### 4. Depth-Limited Search (DLS)
- DFS with a depth limit
- Prevents infinite deep search
- May fail if the limit is too small

### 5. Iterative Deepening DFS (IDDFS)
- Repeated DLS with increasing depth
- Combines DFS space efficiency with BFS completeness

### 6. Bidirectional BFS
- Searches simultaneously from start and goal
- Meets in the middle
- Often faster than standard BFS

---

## 🎨 Visualization Legend

- 🟩 **Green** → Final path  
- 🟨 **Yellow** → Frontier  
- 🟦 **Light Blue** → Explored nodes  
- 🟥 **Red** → Wall  
- 🟢 **Dark Green** → Start (S)  
- 🔵 **Blue** → Target (T)  

---

## 📦 Requirements

Install dependencies before running:

```bash
pip install numpy matplotlib
