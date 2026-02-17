# AI-Pathfinder

AI Pathfinder, Uninformed Search Visualization

This project implements and visualizes multiple uninformed search algorithms on a 10×10 grid environment. The goal is to demonstrate how different "blind" search strategies explore the grid to find a path from the Start node (S) to the Target node (T) while avoiding obstacles.

The visualization shows the frontier, explored nodes, and final path for each algorithm.

Features
10×10 grid environment

Static vertical wall obstacle

Step-by-step visualization using matplotlib

Menu-driven algorithm selection

Parent tracking for path reconstruction

Six search algorithms implemented:

Breadth-First Search (BFS)
Depth-First Search (DFS)
Uniform Cost Search (UCS)
Depth-Limited Search (DLS)
Iterative Deepening DFS (IDDFS)
Bidirectional BFS
Algorithms Implemented
Breadth-First Search (BFS)
Uses a queue (FIFO)
Guarantees shortest path in unweighted grid
Explores level by level
Depth-First Search (DFS)
Uses a stack (LIFO)
Goes deep before backtracking
Does not guarantee shortest path
Uniform Cost Search (UCS)
Uses a priority queue
Expands lowest-cost node first
Optimal for uniform step cost
Depth-Limited Search (DLS)
DFS with depth limit
Prevents infinite deep search
May fail if limit is too small
Iterative Deepening DFS (IDDFS)
Repeated DLS with increasing depth
Combines DFS space efficiency with BFS completeness
Bidirectional BFS
Searches simultaneously from start and goal
Meets in the middle
Faster in many cases
Visualization
🟩 Green → Final path
🟨 Yellow → Frontier
🟦 Light Blue → Explored
🟥 Red → Wall
🟢 Dark Green → Start (S)
🔵 Blue → Target (T)
Requirements
Install dependencies before running:

pip install numpy matplotlib

How to Run
Run via Terminal
Clone the repository:
git clone https://github.com/your-username/ai-pathfinder.git cd ai-pathfinder

Install dependencies:
pip install numpy matplotlib 3. Run the program:

python main.py

Choose an algorithm from the menu when prompted.
Method 2: Run in Jupyter Notebook
If you prefer Jupyter:

Install dependencies (run once in a cell):
!pip install numpy matplotlib

Open main.py and copy the entire code into a Jupyter cell OR place the file in the same directory as the notebook.

Run using:

%run main.py

The visualization window will open and the menu will appear in the output.

Expected Behavior
The grid window opens.
Algorithm exploration is animated.
Final path is highlighted in green.
If no path exists, the search terminates.
