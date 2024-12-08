# Island Perimeter 🏝️

## Project Description

This project implements an algorithm to calculate the perimeter of an island in a 2D grid using a systematic approach to traverse and analyze the grid.

## Implementation Strategy

The solution is developed by following these key steps:

1. **Grid Traversal**
   - Iterate through each cell in the 2D grid systematically
   - Identify land cells (cells with value 1)

2. **Perimeter Calculation Logic**
   - For each land cell, count its exposed edges
   - An edge is considered exposed if:
     - The cell is at the grid's border
     - Adjacent cells are water (value 0)

3. **Edge Counting Method**
   - Check four directions: up, down, left, right
   - Increment perimeter for each water or out-of-bounds adjacent cell
   - This ensures accurate perimeter calculation without double-counting

## Example Implementation Approach

```python
def island_perimeter(grid):
    perimeter = 0
    rows, cols = len(grid), len(grid[0])
    
    for r in range(rows):
        for c in range(cols):
            if grid[r][c] == 1:
                # Check adjacent cells and grid boundaries
                # Count exposed edges
                perimeter += 4 - count_adjacent_land(grid, r, c)
    
    return perimeter
```

## Concepts Covered

- 2D Array (Matrix) manipulation
- Conditional Logic
- Perimeter Calculation
- Grid Navigation
- Algorithmic Problem Solving

## Requirements

- Python 3.4.3
- Ubuntu 20.04 LTS
- PEP 8 Style Guide (version 1.7)

## Example

```python
grid = [
    [0, 0, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0],
    [0, 1, 1, 1, 0, 0],
    [0, 0, 0, 0, 0, 0]
]
print(island_perimeter(grid))  # Output: 12
```

## Constraints

- Grid width and height not exceeding 100
- Grid is rectangular
- Grid is completely surrounded by water
- No "lakes" inside the island

## Learning Objectives

- Understand 2D array traversal
- Apply conditional logic in grid-based problems
- Develop algorithmic thinking for geometric calculations

## Author

Judith
