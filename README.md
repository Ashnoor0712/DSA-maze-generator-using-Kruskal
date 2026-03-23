# Maze Generator using Kruskal’s Algorithm in C++

1. Overview
This project generates a random maze in C++ using Kruskal’s algorithm and the Union-Find (Disjoint Set) data structure. The maze is built from a grid of cells, where walls are removed based on randomly weighted edges while ensuring that the final structure remains connected and acyclic.

The output is displayed as an ASCII maze in the terminal.

2. Features
- Random maze generation on a grid
- Kruskal’s algorithm for building a minimum spanning tree
- Union-Find with path compression and union by rank
- ASCII visualization of the generated maze
- Random edge weights for different maze layouts

3. Concepts Covered
- Graph algorithms
- Kruskal’s algorithm
- Minimum spanning tree
- Union-Find / Disjoint Set
- Path compression
- Union by rank
- Grid graph representation
- Randomized algorithm behavior

4. Tech Stack
- Language: C++
- Standard Libraries:
  - `iostream`
  - `vector`
  - `algorithm`
  - `cstdlib`
  - `ctime`
  - `unordered_set`

5. File Structure
- `main.cpp` — implementation of maze generation using Kruskal’s algorithm

6. How It Works
1. A grid of size `R x C` is treated as a graph
2. Each cell becomes a node
3. Edges are created between neighboring cells
4. Each edge is assigned a random weight
5. Kruskal’s algorithm selects edges in increasing order of weight
6. Union-Find prevents cycles while connecting all cells
7. The final maze is printed in ASCII form

7.  How to Run

Compile the program:

```bash
g++ main.cpp -o program
