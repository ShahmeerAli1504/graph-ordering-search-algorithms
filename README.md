# graph-ordering-search-algorithms

This project solves the **vertex ordering problem** for Bayesian Network learning.  
Given a set of vertices and possible parent sets (with associated costs), the goal is to find an ordering of vertices that minimizes the **total network cost**, using different search strategies.

## Problem Overview
- Each vertex has possible parent sets with a cost.
- An ordering is **consistent** for a vertex if all parents appear before it in the ordering.
- For a given ordering `O`, the cost is the sum of the **minimum consistent parent set costs** for all vertices.
- The task: Find the ordering with the **lowest total cost**.

## Search Algorithms Implemented
- **BFS (Breadth-First Search)** — Explores orderings level by level.
- **DFS (Depth-First Search)** — Explores deeper orderings first.
- **UCS (Uniform-Cost Search)** — Always expands the ordering with the current lowest total cost.

## Features
- Reads dataset files defining:
  - Vertices
  - Possible parent sets
  - Associated costs
- Computes cost for any ordering
- Compares BFS, DFS, and UCS performance
- Outputs:
  - Best ordering found
  - Minimum cost

## How to Run
1. Load the provided dataset into the program.
2. Call the desired search function (`bfs_search`, `dfs_search`, `ucs_search`).
3. View the printed best ordering and total cost.

---
