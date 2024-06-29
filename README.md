# Shortest Path Finder with Visualizer

## Project Overview
This project creates a Shortest Pathfinding Visualizer that helps in understanding pathfinding algorithms step-by-step.

## Project Structure
- Everything related to the this project(i.e., all the code) is located under `/src/PathfindingVisualizer` and `/src/algorithms`.
- The `PathfindingVisualizer` component is imported and rendered in `App.js`.

## How This Project Is Made
### Technologies Used
- **React:** Built using React, a JavaScript library for building user interfaces.
- **JavaScript:** Core programming language used for implementing algorithms and handling logic.
- **CSS:** Styling the components and visual elements of the project.

### Algorithms Implemented
- **Dijkstra's Algorithm:**
  - Dijkstra's algorithm is used for pathfinding in this project. It finds the shortest path between nodes in a graph.
  - **Initialization:** Starts at the start node, setting its distance to 0 and all other nodes' distances to infinity. All nodes are added to a list of unvisited nodes.
  - **Processing Nodes:** Iteratively selects the unvisited node with the smallest known distance. Updates distances to neighbors and marks nodes as visited.
  - **Completion:** Continues until the finish node is reached or there are no more unvisited nodes with finite distances. Reconstructs the shortest path once the finish node is reached.

## Key Functions
- `dijkstra(grid, startNode, finishNode)`: Implements Dijkstra's algorithm to find the shortest path.
- `sortNodesByDistance(unvisitedNodes)`: Sorts unvisited nodes by their distance from the start node.
- `updateUnvisitedNeighbors(node, grid)`: Updates distances of neighboring nodes.
- `getUnvisitedNeighbors(node, grid)`: Retrieves unvisited neighbors of a node.
- `getAllNodes(grid)`: Collects all nodes from the grid.
- `getNodesInShortestPathOrder(finishNode)`: Reconstructs the shortest path from finish node to start node.

## Getting Started
To get started with this project:
- Fork this repository or copy-paste the code.

## Available Scripts
In the project directory, you can run:
- `npm start`: Runs the app in development mode at http://localhost:3000.
- `npm test`: Launches the test runner in interactive watch mode.
- `npm run build`: Builds the app for production to the build folder.
- `npm run eject`: Ejects from Create React App.

Note: Ejecting is a one-way operation that gives full control over project configuration.

