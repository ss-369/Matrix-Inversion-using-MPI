# Matrix-Inversion-using-MPI



## Description

This program computes the **inverse of a matrix** using the row reduction method and distributes the rows of the matrix across multiple processes using MPI.

## Requirements

- **Language**: C/C++ (recommended), Python
- **Framework**: MPI

## Input Format

- The first line contains an integer `N` (dimension of the matrix).
- The next `N` lines contain `N` space-separated floating-point numbers representing the matrix `A`.

## Output Format

- Print the inverse of the matrix with two decimal places.

## Example

### Input
```
3
-2.39 -5.01 -1.32
3.12 3.77 -6.08
5.57 8.44 4.53
```

### Output
```
0.98 0.17 0.51
-0.69 -0.05 -0.27
0.08 -0.11 0.09
```

## How to Run

1. Compile the program:
   ```bash
   mpicc -o matrix_inverse 4.cpp
   ```

2. Run the program with MPI:
   ```bash
   mpiexec -np <number_of_processes> ./matrix_inverse <input_file>
   ```

---

