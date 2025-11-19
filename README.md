# A* Pathfinding Algorithm Visualizer

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pygame](https://img.shields.io/badge/Library-Pygame-yellow.svg)
![Status](https://img.shields.io/badge/Status-Completed-green.svg)

A Python-based interactive application that visualizes the **A* (A-Star) Pathfinding Algorithm** in action. This project demonstrates complex logic, heuristic analysis, and data structure implementation (Priority Queues) to determine the shortest path between two nodes on a grid.

## 🚀 Features

* **Interactive Grid:** Users can draw walls/obstacles with the mouse.
* **Real-time Visualization:** Watch the algorithm scan, evaluate nodes, and backtrack to find the optimal path.
* **Shortest Path Guarantee:** Utilizing the A* logic to ensure the most efficient route is found.
* **Dynamic Reset:** Clear the board or specific nodes instantly.

## 🛠️ Tech Stack

* **Language:** Python 3
* **Library:** Pygame (for rendering the grid and handling user input)
* **Data Structures:** Priority Queues, Hash Sets

## ⚙️ Installation & Usage

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/MrishadK/A-Pathfinding-Visualizer.git
    cd A-Pathfinding-Visualizer
    ```

2.  **Install Dependencies**
    You need `pygame` to run this project.
    ```bash
    pip install pygame
    ```

3.  **Run the Application**
    ```bash
    python main.py
    ```

## 🎮 Controls

| Key / Action | Function |
| :--- | :--- |
| **Left Click** | **First click:** Place Start Node (Orange)<br>**Second click:** Place End Node (Turquoise)<br>**Subsequent clicks:** Draw Barriers (Black) |
| **Right Click** | Erase Node / Barrier |
| **Space Bar** | Start the Algorithm |
| **C Key** | Clear the Grid |

## 🧠 How It Works

The A* algorithm is an informed search algorithm. It searches for the shortest path by combining two cost functions:

$$f(n) = g(n) + h(n)$$

* **$g(n)$:** The cost from the start node to the current node.
* **$h(n)$:** The heuristic (estimated) cost from the current node to the end node.

In this visualization, I used the **Manhattan Distance** as the heuristic function, which is standard for a square grid system allowing 4-directional movement.

### Color Legend
* **Orange:** Start Node
* **Turquoise:** End Node
* **Black:** Barrier (Wall)
* **Green:** Open Nodes (Candidates for exploration)
* **Red:** Closed Nodes (Already visited)
* **Purple:** The Final Shortest Path

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request if you have ideas for improvements (e.g., adding diagonals, different heuristics, or terrain weights).

