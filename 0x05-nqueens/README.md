# 0x05. N Queens

## Description

This project solves the N Queens puzzle using backtracking algorithms.

The N Queens puzzle is the challenge of placing N chess queens on an N×N chessboard so that no two queens threaten each other. Thus, a solution requires that no two queens share the same row, column, or diagonal.

## Tasks

### 0. N queens

Write a program that solves the N queens problem.

* Usage: `nqueens N`
    - where N must be an integer greater or equal to 4
* The program should print every possible solution to the problem
* One solution per line
* Format: see example
* You don't have to print the solutions in a specific order

Example:

```
$ ./0-nqueens 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
```

### 1. N queens - Backtracking

Chess grandmaster Judit Polgár, the strongest female chess player of all time.

Write a program that solves the N queens problem using Backtracking.

* Usage: `nqueens N`
    - where N must be an integer greater or equal to 4
* The program should print every possible solution to the problem
* One solution per line
* Format: see example
* You don't have to print the solutions in a specific order
* You are only allowed to import the `sys` module

Read: [Backtracking](https://en.wikipedia.org/wiki/Backtracking)

```
julien@ubuntu:~/0x08. N Queens$ ./1-nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
julien@ubuntu:~/0x08. N Queens$ ./1-nqueens.py 6
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
[[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
[[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]
julien@ubuntu:~/0x08. N Queens$ 
```

## Usage

To use the N Queens solver:

```
./nqueens N
```

Where `N` is the size of the chessboard.

The program will print all possible solutions to the problem.

## Solution Overview

The backtracking algorithm uses recursion to systematically place queens on the chessboard, one per column. Once a queen is placed, the algorithm checks if the queen is being attacked by any other queen. If so, it backtracks and tries the next position in that column. This continues recursively until a solution is found.

The program prints each valid solution it finds to the standard output.



## Tasks To Complete

+ [x] 0. **N queens**<br/>[0-nqueens.py](0-nqueens.py) contains a script that solves the following challenge:
  + **INFO**: The N queens puzzle is the challenge of placing N non-attacking queens on an N×N chessboard. Write a program that solves the N queens problem.
  + Usage: `nqueens N`:
    + If the user called the program with the wrong number of arguments, print `Usage: nqueens N`, followed by a new line, and exit with the status `1`.
  + Where N must be an integer greater or equal to `4`:
    + If N is not an integer, print `N must be a number`, followed by a new line, and exit with the status `1`.
    + If N is smaller than 4, print `N must be at least 4`, followed by a new line, and exit with the status `1`.
  + The program should print every possible solution to the problem.
    + One solution per line.
    + Format:
      ```ps1
      julien@ubuntu:~/0x08. N Queens$ ./0-nqueens.py 4
      [[0, 1], [1, 3], [2, 0], [3, 2]]
      [[0, 2], [1, 0], [2, 3], [3, 1]]
      julien@ubuntu:~/0x08. N Queens$ ./0-nqueens.py 6
      [[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
      [[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
      [[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
      [[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]
      julien@ubuntu:~/0x08. N Queens$
      ```
    + You don’t have to print the solutions in a specific order.
  + You are only allowed to import the `sys` module.

## Author

Brainstorma - [Github](https://github.com/Brainstorma)
