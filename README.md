# Graph Search in C# (.NET 9.0)

### 📚 CSc 346 – Assignment 4   
**Topic:** Graph ADT, JSON Serialization, DFS & BFS Algorithms  
**Language:** C# (.NET 9.0 Console Application)

---

## 🧠 Overview

This project implements a user-defined **Abstract Data Type (ADT)** in C# to represent and traverse a graph using **Depth First Search (DFS)** and **Breadth First Search (BFS)**.

The graph data is stored in a `.json` file and loaded dynamically at runtime. The app uses **JSON deserialization**, **interface-based design**, and adheres to clean object-oriented principles.

---

## 🔍 Features

- Fully object-oriented design with:
  - `Graph` class
  - `Node` class
  - Interfaces: `IProcessData`, `ISearchAlgorithms`
- Uses `System.Text.Json` for file handling
- DFS and BFS traversal using stack and queue
- Console-based interface for testing
- Example JSON input format included

---

## 📁 File Structure
├── Program.cs ├── Graph.cs ├── Node.cs ├── IProcessData.cs ├── ISearchAlgorithms.cs ├── graphData.json

yaml
Copy
Edit

---

## 📄 Example JSON Format

```json
[
  { "Id": 0, "WasVisited": false, "AdjacentNodes": [1, 2] },
  { "Id": 1, "WasVisited": false, "AdjacentNodes": [0, 3] },
  { "Id": 2, "WasVisited": false, "AdjacentNodes": [0, 3] },
  { "Id": 3, "WasVisited": false, "AdjacentNodes": [1, 2] }
]
▶️ How to Run
Make sure you have .NET 9.0 SDK installed.


dotnet build
dotnet run
Make sure graphData.json is in the root directory or provide the correct path in Program.cs.

🧪 Sample Output
sql
Copy
Edit
Graph Search Program
--------------------
Loaded 4 nodes from JSON.

Depth First Search:
0 1 3 2

Breadth First Search:
0 1 2 3

Search complete.
💡 Notes
This project was developed for academic purposes.

It demonstrates core graph traversal algorithms in a clear, reusable format.

Feel free to fork or contribute if you find it useful!
