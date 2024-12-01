# 0x05. N Queens 👑♟️

## Project Overview 🌟

The N Queens project is a classic algorithmic challenge that tests your problem-solving skills and understanding of backtracking algorithms. The goal is to place N queens on an N×N chessboard such that no two queens threaten each other.

## 🎯 Learning Objectives

By the end of this project, you will:
- Master backtracking algorithms
- Develop recursive problem-solving skills
- Enhance your understanding of chess board configurations
- Improve Python programming techniques

## 🧰 Prerequisites

- Python 3.4.3+
- Basic understanding of:
  - Recursion
  - List manipulations
  - Command-line argument handling

## 🚀 Problem Description

### The Challenge

Place N non-attacking queens on an N×N chessboard. Each solution represents a unique configuration where queens are positioned to avoid:
- Sharing the same row
- Sharing the same column
- Sharing the same diagonal

## 📋 Requirements

### General
- Editors: `vi`, `vim`, `emacs`
- Run on Ubuntu 20.04 LTS
- Follow PEP 8 style guidelines
- First line: `#!/usr/bin/python3`
- Create a `README.md`
- Make files executable

## 🔍 Input Validation

The program must handle the following scenarios:
- ✅ Accept exactly one argument (N)
- ✅ Ensure N is an integer
- ✅ Require N ≥ 4

### Error Handling 🛡️
- Incorrect arguments: `Usage: nqueens N`
- Non-integer input: `N must be a number`
- N < 4: `N must be at least 4`

## 💡 Algorithm Overview

### Key Components
- **Backtracking**: Explore all possible queen placements
- **Recursion**: Systematically try different board configurations
- **Validation**: Check if queens can attack each other

### Solution Approach
1. Start with an empty board
2. Place queens column by column
3. Validate each placement
4. Backtrack if placement is invalid
5. Collect and return all valid solutions

## 🧪 Example Outputs

### 4-Queens
```
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
```

### 6-Queens
```
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
...
```

## 🚦 Usage

```bash
# Run the N Queens solver
./0-nqueens.py 4
./0-nqueens.py 6
```

## 📚 Recommended Resources

- [Backtracking Algorithms](https://www.geeksforgeeks.org/backtracking-algorithms/)
- [Recursion in Python](https://realpython.com/python-recursion/)
- [N Queens Problem Explained](https://www.tutorialspoint.com/data_structures_algorithms/backtracking_algorithms.htm)

## 🏆 Challenges and Learning Opportunities

- Optimize backtracking algorithm
- Minimize computational complexity
- Handle large board sizes efficiently
- Develop robust error handling

## 🤝 Contribution Guidelines

1. Fork the repository
2. Create a feature branch
3. Implement your solution
4. Write comprehensive tests
5. Submit a pull request

## 📝 Notes

- Solutions do not need to be in a specific order
- Focus on correctness and efficiency
- Explore multiple solution strategies

## 🎓 Skills Demonstrated

- Algorithmic thinking
- Recursive problem-solving
- Python programming
- Mathematical reasoning

## ⚖️ Constraints

- Only `sys` module allowed
- No external libraries
- Adhere to project specifications

## 🏅 Inspiration

Inspired by chess grandmaster Judit Polgár, who revolutionized chess strategy and challenged traditional norms.

## 📜 License

Part of the ALX Backend Python curriculum.

---

**Happy Coding! 👩‍💻👨‍💻**
