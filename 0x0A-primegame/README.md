# Prime Game

The goal of the challenge is to implement a function that determines the winner of a game based on a given set of rules.

## Problem Description

The problem involves two players, Alice and Bob, who take turns selecting prime numbers from a given range. The game ends when there are no more prime numbers left in the range. The player with the most prime numbers selected at the end of the game is declared the winner. In case of a tie, the game is declared a draw.

The inputs to the function are as follows:

* `n`: an integer representing the upper limit of the range of numbers to consider
* `prime`: a list of all prime numbers in the range of `1` to `n`

The function should return a string indicating the winner of the game or "Draw" if the game ends in a tie.

## Example

```python
n = 10
prime = [2, 3, 5, 7]

result = prime_game(n, prime)
print(result)
```

Output:

```
Alice
```

## Solution

The `prime_game` function can be implemented using a simple algorithm that keeps track of the number of prime numbers selected by each player. The function should alternate between the two players, starting with Alice, until no more prime numbers are left in the range.

Here's a sample implementation:

```python
def prime_game(n, prime):
    alice = 0
    bob = 0
    
    for i in range(len(prime)):
        if i % 2 == 0:
            alice += 1
        else:
            bob += 1
    
    if alice > bob:
        return "Alice"
    elif bob > alice:
        return "Bob"
    else:
        return "Draw"
```

In this implementation, the `prime_game` function takes in the upper limit of the range `n` and a list of prime numbers `prime`. It initializes the scores for each player to `0` and then loops through the list of prime numbers, incrementing the score for each player alternately.

Finally, the function compares the scores of the two players and returns the winner or "Draw" if the scores are equal.


## Tasks To Complete

+ [x] 0. **Prime Game**<br/>[0-prime_game.py](0-prime_game.py) contains the solution to the following challenge:
  + **INFO:**
    + Maria and Ben are playing a game. Given a set of consecutive integers starting from `1` up to and including `n`, they take turns choosing a prime number from the set and removing that number and its multiples from the set. The player that cannot make a move loses the game.
    + They play `x` rounds of the game, where `n` may be different for each round. Assuming Maria always goes first and both players play optimally, determine who the winner of each game is.
  + **Requirements:**
    + Prototype: `def isWinner(x, nums)`.
    + Where `x` is the number of rounds and `nums` is an array of `n`.
    + Return: name of the player that won the most rounds.
    + If the winner cannot be determined, return `None`.
    + You can assume `n` and `x` will not be larger than 10000.
    + You cannot import any packages in this task.
  + **Example:**
    + `x = 3`, `nums = [4, 5, 1]`
    + First round: `n = 4`.
      + Maria picks 2 and removes 2, 4, leaving 1, 3.
      + Ben picks 3 and removes 3, leaving 1.
      + Ben wins because there are no prime numbers left for Maria to choose.
    + Second round: `n = 5`.
      + Maria picks 2 and removes 2, 4, leaving 1, 3, 5.
      + Ben picks 3 and removes 3, leaving 1, 5.
      + Maria picks 5 and removes 5, leaving 1.
      + Maria wins because there are no prime numbers left for Ben to choose.
    + Third round: `n = 1`
      + Ben wins because there are no prime numbers for Maria to choose.
    + Result: *Ben* has the most wins.

