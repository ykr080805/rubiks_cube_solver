# Rubik's Cube Solver

This project implements a complete solver for the Rubik’s Cube using a variety of algorithmic and object-oriented programming techniques. It combines real-world problem modeling with AI search algorithms and efficient data structures.

## 🔍 Key Learnings from the Project

### 🧩 Modeling Real-World Objects
- Learned how to model a real-world object like the **Rubik’s Cube** in a way that is understandable and computable for a computer.
- Understood how to represent the cube's states and transitions effectively using classes and data structures.

### 🧠 Problem Decomposition
- Learned how to break down a large problem like a Rubik’s Cube solver into smaller manageable modules such as:
    - Rubik’s Cube representation
    - Solvers and search algorithms
    - Pattern database generation and usage

### 🧱 Object-Oriented Design
- Applied Object-Oriented Programming principles to design flexible and extensible systems:
    - **Base Classes**: Created base classes for the Rubik’s Cube and Pattern Databases
    - **Class Hierarchy**: Used inheritance and polymorphism to build reusable components
    - **Operator Overloading**: Enabled intuitive comparison and hashing of cube states

#### Concepts Used:
- Classes and Objects
- Inheritance
- Virtual Functions and Abstract Classes
- Operator Overloading

### 🔄 Algorithmic Techniques
- Studied and applied classical pathfinding algorithms:
    - **Breadth-First Search (BFS)**
    - **Depth-First Search (DFS)**
    - **Iterative Deepening DFS (IDDFS)**
    - **Iterative Deepening A* (IDA\*)**
- Learned how these algorithms apply to real-world AI problems like Rubik’s Cube solving.

### 🧠 Heuristic Search
- Implemented **A\*** and **IDA\*** with **Pattern Databases** to enable efficient heuristic search.
- Understood how precomputing optimal moves and storing them enables rapid solving.

## 🛠 Miscellaneous Technical Learnings
- How `unordered_map<>` works with custom objects
- How to create custom hash functions for efficient lookup
- How to store information using bit manipulation
- Techniques to **save and load** data to and from files
- Explored the concept of **Black Boxing**: giving an input to a system and expecting a defined output (e.g., using a Permutation Indexer)

---
## 📁 Project Structure
rubiks_cube_solver/
├── cmake-build-debug/ # Build directory (auto-generated)
├── Databases/
│ └── cornerDepth5V1.txt # Precomputed pattern database
├── Model/
│ ├── PatternDatabase/
│ │ ├── RubiksCube.h/.cpp
│ │ ├── RubiksCube1dArray.cpp
│ │ ├── RubiksCube3dArray.cpp
│ │ └── RubiksCubeBitboard.cpp
│ └── PatternDatabases/
│ ├── CornerDBMaker.h/.cpp
│ ├── CornerPatternDatabase.h/.cpp
│ ├── PatternDatabase.h/.cpp
│ ├── math.h/.cpp
│ ├── NibbleArray.h/.cpp
│ └── PermutationIndexer.h
├── Solver/
│ ├── BFSSolver.h
│ ├── DFSSolver.h
│ ├── IDAstarSolver.h
│ └── IDDFSSolver.h
├── main.cpp # Program entry point
├── CMakeLists.txt # CMake build configuration
└── readme.md


---

## 🧩 What We Learned

### ✅ Modeling & Decomposition
- Represented a real-world object (Rubik's Cube) in code.
- Decomposed the solver into modules: representation, heuristics, search, etc.

### ✅ Object-Oriented Programming
- Created base and derived classes for cube states and solvers.
- Applied OOP concepts:
    - Classes and Objects
    - Virtual Functions & Abstract Classes
    - Inheritance
    - Operator Overloading

### ✅ AI & Algorithms
- Implemented search algorithms:
    - BFS, DFS, IDDFS, IDA*
- Built and used **Pattern Databases** for heuristic guidance.
- Applied **Heuristic Search Algorithms** like A* and IDA* effectively.

### ✅ Technical Skills
- Custom `unordered_map` hashing
- Bit manipulation for space-efficient storage
- File I/O for pattern database loading
- Black-box abstraction (Permutation Indexer)

---

## 🛠️ Build Instructions

### 🧰 Requirements:
- C++17 compatible compiler (e.g. GCC, Clang, MSVC)
- CMake ≥ 3.10

### 🧪 Build Steps:

```bash
# Clone the repository
git clone https://github.com/yourusername/rubiks_cube_solver.git
cd rubiks_cube_solver

# Create build directory and compile
mkdir build && cd build
cmake ..
make

# Run the solver
./rubiks_cube_solver

