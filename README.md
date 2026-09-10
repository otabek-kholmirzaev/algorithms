# Algorithms

A collection of **data structures and graph algorithms implemented in C#**, with a focus on understanding core algorithmic techniques through concise, runnable examples.

The repository contains implementations and practice problems covering graph traversal, shortest paths, disjoint-set data structures, and tree algorithms.

## Implemented

| Topic                          | Implementation  | Notes                                 |
| ------------------------------ | --------------- | ------------------------------------- |
| **Breadth-First Search (BFS)** | `BFS/`          | Queue-based graph traversal           |
| **Depth-First Search (DFS)**   | `DFS/`          | Stack-based graph traversal           |
| **Dijkstra's Algorithm**       | `Djkstra/`      | Shortest paths using a priority queue |
| **Union-Find**                 | `UnionFind/`    | Disjoint-set data structure           |
| **Tree Problems**              | `DFS/Problems/` | DFS-based LeetCode solutions          |

## Algorithms

### Breadth-First Search

`BFS/Program.cs` demonstrates BFS on an adjacency-list graph using:

* `Queue<T>`
* `HashSet<T>`
* Adjacency-list graph representation

```text
A
├── C
└── E
```

BFS is useful for level-order traversal and finding shortest paths in **unweighted graphs**.

**Time:** `O(V + E)`
**Space:** `O(V)`

The implementation uses a queue and visited set to traverse the graph.

### Depth-First Search

`DFS/Program.cs` demonstrates iterative DFS using:

* `Stack<T>`
* `HashSet<T>`
* Adjacency-list graph representation

**Time:** `O(V + E)`
**Space:** `O(V)`

The repository also contains DFS-based tree problem solving under:

```text
DFS/Problems/
└── Number of Good Leaf Nodes Pairs.cs
```

The solution applies DFS to collect root-to-leaf paths and then evaluates distances between leaf nodes.

### Dijkstra's Algorithm

The `Djkstra/` project contains a solution for the LeetCode **Network Delay Time** problem.

The implementation uses:

* Adjacency lists
* `PriorityQueue<TElement,TPriority>`
* Distance relaxation
* Visited-node tracking

**Time:** `O((V + E) log V)`
**Space:** `O(V + E)`

The algorithm returns the maximum shortest-path distance from the source, or `-1` when some nodes are unreachable.

### Union-Find

The `UnionFind/` directory is reserved for implementations and problems involving the **Disjoint Set Union (DSU)** data structure.

Typical applications include:

* Dynamic connectivity
* Connected components
* Cycle detection
* Minimum spanning trees
* Kruskal's algorithm

The implementation is currently a work in progress.

## Project Structure

```text
algorithms/
├── BFS/
│   ├── BFS.csproj
│   ├── Program.cs
│   └── graph.png
│
├── DFS/
│   ├── DFS.csproj
│   ├── Program.cs
│   ├── graph.png
│   └── Problems/
│       └── Number of Good Leaf Nodes Pairs.cs
│
├── Djkstra/
│   ├── Djkstra.csproj
│   ├── Program.cs
│   └── Solution.cs
│
├── UnionFind/
│   ├── UnionFind.csproj
│   ├── Program.cs
│   └── UnionFind.cs
│
├── algorithms.sln
├── LICENSE
└── README.md
```

The repository is organized as separate .NET console projects so individual algorithms can be studied and executed independently.

## Tech Stack

* **C#**
* **.NET 8**
* **Visual Studio / .NET CLI**

Each implemented algorithm project targets `net8.0` and uses nullable reference types and implicit global usings.

## Getting Started

### Prerequisites

Install the [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0).

### Clone

```bash
git clone https://github.com/otabek-kholmirzaev/algorithms.git
cd algorithms
```

### Run an algorithm

For example, run BFS:

```bash
cd BFS
dotnet run
```

DFS:

```bash
cd DFS
dotnet run
```

Dijkstra:

```bash
cd Djkstra
dotnet run
```

## Learning Goals

This repository is primarily used to practice and reinforce:

* Graph representation
* Graph traversal
* Shortest-path algorithms
* Trees and recursion
* Data structures
* Algorithmic complexity
* Competitive programming techniques
* Translating algorithmic ideas into clean C# implementations

## Future Additions

Planned topics include:

* Union-Find / DSU
* Kruskal's algorithm
* Prim's algorithm
* Topological sorting
* Minimum spanning trees
* Bellman-Ford
* Floyd-Warshall
* Binary search
* Dynamic programming
* Backtracking
* More tree and graph problems

## License

This project is licensed under the **MIT License**.
