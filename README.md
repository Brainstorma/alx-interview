# 0x00. Pascal's Triangle

This project contains the implementation of a program that prints Pascal's triangle up to a specified number of rows.

The program takes an integer argument, `n`, which represents the number of rows to generate in Pascal's triangle. It then prints Pascal's triangle up to the `n`th row.

## Tasks To Complete

+ [x] 0. **Pascal's Triangle**<br/>[0-pascal_triangle.py](0-pascal_triangle.py) contains a function `def pascal_triangle(n):` that returns a list of lists of integers representing the Pascal's triangle of `n`:
  + Returns an empty list if `n <= 0`.
  + You can assume `n` will be always an integer.

## Usage
To compile the program, use the following command:
```
gcc -Wall -Werror -Wextra -pedantic pascal_triangle.c main.c -o pascal
```

To run the program, use the following command:
```
./pascal <n>
```
Replace `<n>` with the number of rows you want to generate in Pascal's triangle.

## Examples
```
$ ./pascal 5
          1
        1   1
      1   2   1
    1   3   3   1
  1   4   6   4   1
```

```
$ ./pascal 0
```

## Algorithm
To generate Pascal's triangle, we can use a 2D array to store the triangle. Each cell in the triangle will correspond to a number in Pascal's triangle.

To generate Pascal's triangle, we can use a nested loop. The outer loop will iterate over the rows of the triangle, while the inner loop will iterate over the columns of the triangle.

The value of each cell in the triangle can be calculated based on the values of the cells in the previous row. Specifically, the value of each cell can be calculated by summing the values of the cells directly above and to the left of it.

To handle the edge cases (first and last column of each row), we will initialize these values to 1. The first and last row will also be initialized to 1.

## Implementation Details
The program is implemented in C.

The program consists of two files:
1. `pascal_triangle.c`: This file contains the implementation of the function `pascal_triangle()`, which generates Pascal's triangle up to a specified number of rows.
2. `main.c`: This file contains the main function, which accepts the number of rows as a command-line argument and calls the `pascal_triangle()` function to generate and print Pascal's triangle.

The `pascal_triangle()` function takes an integer argument, `n`, which represents the number of rows to generate in Pascal's triangle. It allocates memory for a 2D array to store the triangle, calculates the values of each cell in the triangle, and prints the triangle.

The `main()` function accepts the number of rows as a command-line argument, converts it to an integer, and calls the `pascal_triangle()` function to generate and print Pascal's triangle.

## Files
- `pascal_triangle.c`
- `main.c`
- `pascal` (executable)

## How to use it? 🧩
When you execute the script it will print Pascal's Triangle with 10 levels, for exited the script please press `q`. The output will be like this:

```bash
$ ./pascal
                              1
                          1       1
                      1       2       1
                  1       3       3       1
              1       4       6       4       1
          1       5       10      10      5       1
      1       6       15      20      15      6       1
  1       7       21      35      35      21      7       1
1       8       28      56      70      56      28      8       1
If you want to quit the program press 'q': 0
$
```

```bash
$ ./pascal
                              1
                          1       1
                      1       2       1
                  1       3       3       1
              1       4       6       4       1
          1       5       10      10      5       1
      1       6       15      20      15      6       1
  1       7       21      35      35      21      7       1
1       8       28      56      70      56      28      8       1
If you want to quit the program press 'q': 5
                          1
                      1       1
                  1       2       1
              1       3       3       1
          1       4       6       4       1
$
```

```bash
$ ./pascal
                              1
                          1       1
                      1       2       1
                  1       3       3       1
              1       4       6       4       1
          1       5       10      10      5       1
      1       6       15      20      15      6       1
  1       7       21      35      35      21      7       1
1       8       28      56      70      56      28      8       1
If you want to quit the program press 'q': 10
                                          1
                                      1       1
                                  1       2       1
                              1       3       3       1
                          1       4       6       4       1
                      1       5       10      10      5       1
                  1       6       15      20      15      6       1
              1       7       21      35      35      21      7       1
          1       8       28      56      70      56      28      8       1
      1       9       36      84     126     126      84      36      9       1
  1       10      45      120     210     252     210      120     45      10      1

``` 

## How to test it with Unit Test? 🧪

1. Compile the script with the next command:
```bash
make test
```
