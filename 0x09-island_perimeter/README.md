# 0x09 Island Perimeter

Welcome to the "0x09 Island Perimeter" project repository! This project focuses on solving the island perimeter problem, where you're given a 2D grid representing an island, and you need to calculate its perimeter. Below, you'll find an overview of the main project and a link to the task repository.

## Main Project Overview

### Project Description
The "0x09 Island Perimeter" project aims to develop a solution to the island perimeter problem, a classic algorithmic problem in computer science. Given a 2D grid where '1's represent land and '0's represent water, the goal is to calculate the perimeter of the island formed by connecting adjacent land cells.

### Problem Statement
You are given a 2D grid, where 1's are representing land and 0's are representing water. You need to calculate the perimeter of the island, where the perimeter is defined by the number of edges that connect land cells to water cells or the boundary of the grid.

### Project Structure
This repository contains the code for solving the island perimeter problem. The solution will involve designing an efficient algorithm to traverse the grid and calculate the perimeter based on the given rules.

## Tasks To Complete

+ [x] 0. **Island Perimeter**<br/>[0-island_perimeter.py](0-island_perimeter.py) contains a module with a function having the prototype `function def island_perimeter(grid):`, which returns the perimeter of the island described in `grid`, with the following requirements:
  + `grid` is a list of list of integers:
    + 0 represents water.
    + 1 represents land.
    + Each cell is square, with a side length of 1.
    + Cells are connected horizontally/vertically (not diagonally).
    + `grid` is rectangular, with its width and height not exceeding 100.
  + The grid is completely surrounded by water.
  + There is only one island (or nothing).
  + The island doesn't have "lakes' (water inside that isn't connected to the water surrounding the island).

