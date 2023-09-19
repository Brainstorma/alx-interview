# 0x08-making_change

## Project Description

This project is part of the ALX curriculum and focuses on solving the "Making Change" problem. The goal of this project is to develop an algorithm in Python that calculates the minimum number of coins needed to make change for a given amount using a predefined set of coin denominations. This project is designed to help you improve your understanding of dynamic programming and algorithmic problem-solving.

## Task

The main task for this project can be found [here](https://link-to-task-description.com/0x08-making-change-task). In summary, the task requires you to implement a Python function that takes two parameters: the `amount` to make change for and a list of `denominations` representing the available coin values. The function should return the minimum number of coins needed to make change for the given amount using the provided denominations.

## Getting Started

To get started with this project, follow these steps:

1. Clone this repository to your local machine:

    ```shell
    git clone https://github.com/brainstorma/0x08-making_change.git
    ```

2. Navigate to the project directory:

    ```shell
    cd 0x08-making_change
    ```

3. You can now start working on the project and implementing the required functionality.

## Usage

You can use the provided Python script to test your implementation. Here's how you can use it:

1. Import the `makeChange` function from `make_change.py` into your Python script:

    ```python
    from make_change import makeChange
    ```

2. Use the `makeChange` function to calculate the minimum number of coins needed:

    ```python
    amount = 25
    denominations = [1, 10, 25]
    result = makeChange(amount, denominations)
    print(f"Minimum number of coins needed: {result}")
    ```

3. Execute your Python script.

## Contributing

Contributions to this project are welcome! If you have any improvements, bug fixes, or additional features to propose, please create a pull request. Be sure to follow the [contributing guidelines](CONTRIBUTING.md) for this project.


## Tasks To Complete

+ [x] 0. **Change comes from within**<br/>[0-making_change.py](0-making_change.py) contains a module with a function that determines the fewest number of coins needed to meet a given amount `total` when given a pile of coins of different values, with the following requirements:
  + Prototype: `def makeChange(coins, total)`.
  + Return: fewest number of coins needed to meet `total`.
    + If `total` is `0` or less, return `0`.
    + If `total` cannot be met by any number of coins you have, return `-1`.
  + `coins` is a list of the values of the coins in your possession.
  + The value of a coin will always be an integer greater than `0`.
  + You can assume you have an infinite number of each denomination of coin in the list.
  + Your solution’s runtime will be evaluated in this task.

