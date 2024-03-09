# TRANSPORT-PATH-ANALYSIS

TRANSPORT PATH ANALYSIS is a Python project designed to analyze and compare various pathfinding algorithms in transportation scenarios. This project explores different algorithms to find the shortest routes between cities in a customizable graph, considering factors such as distance and travel time.

## Purpose

The purpose of this project is to evaluate the performance of different pathfinding algorithms commonly used in transportation route planning. By implementing and comparing algorithms such as Depth-First Search (DFS), Breadth-First Search (BFS), Best-First Search, and A* Search, users can gain insights into the efficiency and effectiveness of each approach in finding optimal routes.

## Functionality

- **Graph Creation**: Allows users to define custom transportation scenarios by specifying cities and their connections (highways and railways) along with distances and travel times.
  
- **Algorithm Implementation**: Implements DFS, BFS, Best-First Search, and A* Search algorithms to find the shortest paths between specified start and goal cities within the transportation scenario graph.

- **Visualization**: Visualizes the transportation scenario graph with highlighted shortest paths for each algorithm, providing a clear understanding of the route planning process.

- **Performance Comparison**: Measures and compares execution times and path lengths for each algorithm, enabling users to evaluate their efficiency in route optimization.

## Implemented Algorithms

### Depth-First Search (DFS)
- **Purpose**: DFS aims to explore as far as possible along each branch before backtracking, effectively traversing the graph depth-first.
- **Functionality**: Starting from the specified start city, DFS explores each possible path until it reaches the goal city, using a stack data structure to track nodes.
- **Analysis**: While DFS is memory efficient, it may not always find the shortest path due to its nature of exploring one branch completely before moving on.
- **Results**: DFS returns a path between the start and goal cities, which may not be the shortest but is one of the possible paths.

### Breadth-First Search (BFS)
- **Purpose**: BFS systematically explores all neighbor nodes at the present depth before moving to the next depth level, ensuring the shortest path is found first.
- **Functionality**: BFS explores the graph level by level, utilizing a queue data structure to track nodes and prioritize exploration.
- **Analysis**: BFS guarantees finding the shortest path in unweighted graphs, making it suitable for scenarios prioritizing shortest path discovery.
- **Results**: BFS returns the shortest path between the start and goal cities in terms of the number of edges traversed.

### Best-First Search
- **Purpose**: Best-First Search is a heuristic search algorithm that prioritizes nodes based on an evaluation function, aiming to reach the goal faster.
- **Functionality**: Using a priority queue, Best-First Search explores nodes based on a heuristic evaluation, guiding the search towards the goal efficiently.
- **Analysis**: Best-First Search combines advantages of BFS and heuristic search, providing near-optimal solutions depending on the accuracy of the heuristic function.
- **Results**: The algorithm returns a path close to the shortest, considering the heuristic estimate.

### A* Search
- **Purpose**: A* Search combines Dijkstra's algorithm and Best-First Search, incorporating both the cost of reaching a node and a heuristic estimate of the cost to reach the goal.
- **Functionality**: A* Search explores nodes by considering the total cost from the start and the estimated cost to reach the goal, using a priority queue to prioritize nodes.
- **Analysis**: A* Search is optimal and complete when both the cost and heuristic functions are admissible, making it suitable for scenarios requiring the shortest path efficiently.
- **Results**: A* Search returns the shortest path between the start and goal cities, considering both edge costs and heuristic estimates.

## Usage

1. **Installation**: Clone the repository to your local machine.

2. **Dependencies**: Make sure you have Python installed along with the required libraries (NetworkX, Matplotlib).

3. **Customization**: Modify the `create_custom_scenario_graph()` function to define your transportation scenario.

4. **Execution**: Run the desired algorithm functions (`dfs_shortest_path_scenario`, `bfs_shortest_path_scenario`, `best_first_search_scenario`, `astar_search`) with appropriate start and goal cities.

5. **Visualization**: View the generated plots to visualize the transportation scenario graph and highlighted shortest paths.

6. **Performance Analysis**: Compare execution times and path lengths for each algorithm to evaluate their effectiveness.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

