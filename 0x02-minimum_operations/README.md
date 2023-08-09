# 0x02. Minimum Operations 

## Description

This project involves writing a program to calculate the minimum number of operations needed to result in exactly `n` `H` characters in the text. 

The only operations allowed are:

- Copy All
- Paste

## Usage

The program can be run like:
./minoperations n


Where `n` is the number of `H` characters desired in the final text. 

The program will print the minimum number of operations required.

## Tasks

- [ ] 1. Main file - Write a [main file](./0-minoperations.py) that tests the `minOperations` function. It should call the function with different values of `n` and print the returned output. Add edge cases like `n = 0` or `n = impossible`.


## Tasks To Complete

+ [x] 0. **Minimum Operations**<br/>[0-minoperations.py](0-minoperations.py) contains a script that meets the following requirements:
  + In a text file, there is a single character `H`. Your text editor can execute only two operations in this file: `Copy All` and `Paste`. Given a number `n`, write a method that calculates the fewest number of operations needed to result in exactly `n` `H` characters in the file.
    + Prototype: `def minOperations(n)`.
    + `boxes` is a list of lists.
    + Returns an integer.
    + If `n` is impossible to achieve, return `0`.

