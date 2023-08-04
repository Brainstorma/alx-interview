# 0x01. Lockboxes

This project is about opening a series of lockboxes using keys found in previous lockboxes.

## Description

You have n number of locked boxes in front of you. Each box is numbered sequentially from 0 to n - 1 and each box may contain keys to the other boxes. 

Write a method that determines if all the boxes can be opened.

* Prototype: def canUnlockAll(boxes)
* boxes is a list of lists
* A key with the same number as a box opens that box
* You can assume all keys will be positive integers
* The first box boxes[0] is unlocked
* Return True if all boxes can be opened, else return False

## Tasks

* 0. Lockboxes
  * Write a method that determines if all the boxes can be opened.

* 1. Helper function
  * Write a method that checks if a key matches a box.

* 2. Key checker
  * Write a method that checks if a key opens a box.

## Usage

```python
boxes = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]] 

print(canUnlockAll(boxes))
# True

## Tasks To Complete

+ [x] 0. **Lockboxes**<br/>[0-lockboxes.py](0-lockboxes.py) contains a script that meets the following requirements:
  + You have `n` number of locked boxes in front of you. Each box is numbered sequentially from `0` to `n - 1` and each box may contain keys to the other boxes.
  + Write a method that determines if all the boxes can be opened.
    + Prototype: `def canUnlockAll(boxes)`.
    + `boxes` is a list of lists.
    + A key with the same number as a box opens that box.
    + You can assume all keys will be positive integers.
      + There can be keys that do not have boxes.
    + The first box `boxes[0]` is unlocked.
    + Return `True` if all boxes can be opened, else return `False`.

