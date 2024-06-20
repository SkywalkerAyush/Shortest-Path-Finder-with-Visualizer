Pathfinding Visualizer Tutorial
This project is a tutorial for creating a Pathfinding Visualizer. It visualizes pathfinding algorithm and helps in understanding how they work step-by-step.

Project Structure
Everything related to the tutorial (i.e., all the code) is located under /src/PathfindingVisualizer and /src/algorithms. The PathfindingVisualizer component is imported and rendered in App.js.

How This Project Is Made
Technologies Used
React: This project is built using React, a JavaScript library for building user interfaces.
JavaScript: The core programming language used for implementing the algorithms and handling logic.
CSS: Styling the components and visual elements of the project.
Algorithm Implemented
Dijkstra's Algorithm
Dijkstra's algorithm is the primary algorithm used in this project for pathfinding. It is a popular algorithm for finding the shortest path between nodes in a graph. Here's a detailed explanation of how it works:

Initialization:

The algorithm starts at the given start node, setting its distance to 0 and all other nodes' distances to infinity.
All nodes are added to a list of unvisited nodes.
Processing Nodes:

The algorithm processes nodes by iteratively selecting the unvisited node with the smallest known distance.
If this node's distance is infinity, the algorithm terminates as there are no more reachable nodes.
The selected node is marked as visited and added to the list of visited nodes in order.
Updating Neighbors:

For the selected node, the algorithm calculates the tentative distances to each of its unvisited neighbors.
If the calculated distance to a neighbor is smaller than its current known distance, the neighbor's distance is updated, and its previous node is set to the current node.
Completion:

The algorithm continues processing nodes until it reaches the finish node or there are no more unvisited nodes with finite distances.
Once the finish node is reached, the algorithm reconstructs the shortest path by following the previous nodes from the finish node back to the start node.
Key Functions
dijkstra(grid, startNode, finishNode):

Implements Dijkstra's algorithm to find the shortest path from the start node to the finish node.
Manages the list of unvisited nodes, selects the closest node, and updates neighbors' distances.
sortNodesByDistance(unvisitedNodes):

Sorts the list of unvisited nodes by their current known distance from the start node.
updateUnvisitedNeighbors(node, grid):

Updates the distances of the neighboring nodes of the current node.
getUnvisitedNeighbors(node, grid):

Retrieves all the neighbors of a node that have not yet been visited.
getAllNodes(grid):

Collects all nodes from the grid into a single list, which is used to initialize the list of unvisited nodes.
getNodesInShortestPathOrder(finishNode):

Reconstructs the shortest path from the finish node back to the start node by following the previous nodes.
Getting Started
To get started with this project, you can fork this repository or copy-paste the code.

Available Scripts
In the project directory, you can run:

npm start
Runs the app in development mode.<br>
Open http://localhost:3000 to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

npm test
Launches the test runner in interactive watch mode.<br>
See the section about running tests for more information.

npm run build
Builds the app for production to the build folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about deployment for more information.

npm run eject
Note: this is a one-way operation. Once you eject, you can’t go back!

If you aren’t satisfied with the build tool and configuration choices, you can eject at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc.) right into your project so you have full control over them. All of the commands except eject will still work, but they will point to the copied scripts so you can tweak them. At this point, you’re on your own.

You don’t have to ever use eject. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However, we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

