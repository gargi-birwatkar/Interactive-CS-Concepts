# Shortest Path Algorithms Visualizer

## 🌐 About This Simulation

This interactive tool is a dynamic graph visualization environment designed to demonstrate how various **Shortest Path Algorithms** find the optimal route between two points in a weighted graph.

It transforms abstract algorithm theory into clear, step-by-step visual processes, making it an excellent resource for learning and teaching graph traversal concepts.

## 🧠 Key Algorithms Visualized

This simulation allows you to choose from and execute several fundamental graph algorithms:

| Algorithm | Description | Best For |
| :--- | :--- | :--- |
| **Breadth-First Search (BFS)** | Finds the shortest path in an **unweighted** graph. | Determining the minimum number of edges to reach a destination. |
| **Dijkstra's Algorithm** | Finds the shortest path in a graph with **non-negative** edge weights. | Calculating the lowest cost or shortest time path. |
| **Bellman-Ford Algorithm** | Finds the shortest path in a graph that may contain **negative** edge weights. | Identifying and handling negative cycles in a network. |
| **A\* Search Algorithm** | An extension of Dijkstra's that uses a heuristic (estimated cost) to significantly **speed up** pathfinding. | Practical applications like game AI and route planning. |

## ⚙️ Features and Usage

### Visualization Highlights

* **Node States:** Watch nodes change color as they are **Visited**, added to the **Frontier** (the priority queue or queue), or confirmed as part of the **Final Path**.
* **Distance Updates:** Observe the distance values associated with each node change in real-time as the algorithm finds shorter paths.
* **Weighted Edges:** Interact with a graph where edges have defined weights (costs).

### Getting Started

You can run this simulation easily in any modern web browser.

1.  Navigate to the directory containing `algo_visualization.html`.
2.  Open the file `algo_visualization.html` in your web browser.

### Controls

| Control | Function |
| :--- | :--- |
| **Algorithm Dropdown** | Select the algorithm you wish to run (e.g., Dijkstra's, A\*). |
| **Start/End Nodes** | Click on any two nodes in the graph to designate the starting point and the target destination. |
| **Run Button** | Executes the entire algorithm at the speed defined by the slider. |
| **Step Button** | Executes one logical step of the algorithm at a time, perfect for tracing the logic. |
| **Speed Slider** | Controls the delay between steps for visual inspection. Set to **0** for step-by-step mode. |
| **Reset Button** | Clears the graph state, allowing you to select a new algorithm or new start/end points. |

## 💻 Technical Details

* **File:** `algo_visualization.html`
* **Technology:** HTML, CSS, and JavaScript.
* **Target Audience:** Students and educators focused on Data Structures and Algorithms.
