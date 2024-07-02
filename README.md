# Heap-Management-System

This project demonstrates the implementation of garbage collection using the mark-and-sweep method in C. The program manages a graph-like structure with nodes, where each node can point to up to three other nodes. The garbage collection mechanism ensures that only nodes reachable from the root nodes are kept, while unreachable nodes are identified and deallocated.

## Features

1. **Initialization of Nodes**
   - Initializes an array of 8 nodes with predefined values.
   - Sets up reference counts and mark flags for each node.

2. **Edge Setup**
   - Establishes edges between nodes to form a directed graph.

3. **Print Nodes**
   - Displays the data, reference count, and memory size of each node.

4. **Adjacency List and Matrix**
   - Provides both adjacency list and adjacency matrix representations of the graph.

5. **Mark and Sweep**
   - Implements mark-and-sweep garbage collection to identify and free unreachable nodes.

## Usage

1. Compile the program using a C compiler.
2. Run the executable.
3. The program will initialize the nodes, set up edges, and display the graph's adjacency list and matrix.
4. It then performs mark-and-sweep garbage collection and displays the updated adjacency list and matrix.

## Functions

- `print_node(int i)`: Prints the data, reference count, and freed size of a node.
- `edgeSet(int so, int dest1, int dest2, int dest3)`: Sets edges between nodes.
- `print_allNodes(Node* root)`: Prints all nodes reachable from a given root node.
- `adjacency_list()`: Displays the adjacency list of the graph.
- `root_is_present(Node* root_1, Node* temp)`: Checks if a node is present in the root's list.
- `reference_counting(Node* root)`: Decrements reference counts and frees memory for unreachable nodes.
- `adjacency_Matrix()`: Displays the adjacency matrix of the graph.
- `mark_the_Nodes(Node* root, int i, int j)`: Marks nodes as reachable.
- `mark_method(Node* root)`: Marks all reachable nodes starting from a given root node.
- `sweep_method()`: Frees memory for nodes that are not marked as reachable.

This project showcases the fundamentals of garbage collection using the mark-and-sweep technique, ensuring efficient memory management in a graph structure.
