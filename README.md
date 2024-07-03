# Heap-Management-System

This project simulates a basic memory management system. It allows for allocating and freeing memory, displaying current memory allocations and free memory blocks, and merging free memory blocks. The program is implemented in C using linked lists to represent allocated and free memory blocks.

## Features

1. **Allocate Memory**: Requests a specified amount of memory and allocates it if available.
2. **Free Memory**: Frees memory blocks previously allocated.
3. **Display Memory Stats**: Shows the current status of both allocated and free memory blocks.
4. **Merge Free Blocks**: Combines adjacent free memory blocks to create larger contiguous blocks.

## Components

- **Allocated Memory Nodes (nodea)**:
  - `char data[5]`: Identifier for the memory block.
  - `int address`: Starting address of the memory block.
  - `int memory`: Size of the memory block.
  - `struct nodealloc *next`: Pointer to the next allocated memory block.

- **Free Memory Nodes (nodef)**:
  - `int start_address`: Starting address of the free memory block.
  - `int end_address`: Ending address of the free memory block.
  - `int memory`: Size of the free memory block.
  - `struct nodefree *next`: Pointer to the next free memory block.

## Functions

- **Node Creation**: Functions to create nodes for allocated and free memory lists.
- **Insertion**: Functions to insert nodes at the start of allocated and free memory lists.
- **Display**: Functions to print the current allocated and free memory lists.
- **Memory Allocation**: Function to allocate memory and modify the free memory list.
- **Memory Deallocation**: Function to free memory and update the free memory list.
- **Merge Free Blocks**: Function to merge two lists of free memory blocks.

## Usage

The program provides a menu-driven interface to:
1. Allocate memory.
2. Free memory.
3. Display current memory allocations and free blocks.
4. Exit the program.

This project demonstrates a simplified memory management approach suitable for educational purposes.
