# Informed-Search

Informed Search, also known as Heuristic Search, is a type of search algorithm that uses domain-specific knowledge (heuristics) to find solutions more efficiently than uninformed search methods. This repository demonstrates two popular informed search algorithms:

## 1. A* (A-Star) Search
A* Search combines the benefits of both Uniform Cost Search and Greedy Best-First Search. It uses:
- Path cost from start node (g(n))
- Heuristic estimate to goal (h(n))
- Total cost f(n) = g(n) + h(n)

Features:
- Complete: Always finds a solution if one exists
- Optimal: Guarantees the shortest path
- More efficient than uninformed search algorithms

## 2. Greedy Best-First Search
A search algorithm that uses heuristic function to estimate the cost from current node to goal. It:
- Always expands the node closest to the goal
- Makes locally optimal choices
- Is faster but doesn't guarantee the shortest path

### Implementation Details
Both algorithms are implemented using:
- Priority Queue for frontier management
- Dictionary/HashMap for graph representation
- Heuristic functions for distance estimation

### Example Graph Structure
The implementations use a graph with:
- Nodes: S (Start), A, B, C, D, G (Goal)
- Heuristic values for each node
- Edge connections with associated costs (for A*)

### Usage
The repository contains Jupyter notebooks demonstrating both algorithms:
- `a_star_search.ipynb`: Implementation of A* Search
- `greedy_best_first_search.ipynb`: Implementation of Greedy Best-First Search

Each notebook includes:
- Algorithm implementation
- Graph representation
- Example execution with results
