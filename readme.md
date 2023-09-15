# SRC scholarship test

## Problem
You need to implement operations for square sparse matrices stored in a row major format:
- Matrix multiplication.
- Raising to an integer power `p`.

## Matrix format
- `SparseMatrix` is a list/vector of (sorted!) list/vectors of `Element`-s.
- `Element` has index and value of a non-zero element.

**Example.** `[[Element(1, 5)], [Element(0, 3)]]` corresponds to the matrix [[0, 5], [3, 0]].

## Tasks
### C++
Requirements: CMake, C++17 compiler. Implement:
1. `SparseMatrix SparseMatrix::operator*(const SparseMatrix &m)`.
2. `SparseMatrix SparseMatrix::operator^(uint32_t p)`.
### Python
Requirements: Python >= 3.9 interpreter. Implement:
1. `SparseMatrix.__matmul__(self, other)`.
2. `SparseMatrix.__pow__(self, power, modulo=None)` (ignore `modulo` argument).

**Note.** There is a sample code, you need to replace it.

## Testing
To test, compile and run the project (C++) or run `main.py` (Python).
- `check_power_2`: tests squaring the matrix using `operator*`/`__matmul__`.
- `check_power_5`: tests raiding to the 5th power using `operator^`/`__pow__`.
- `check_power_999`: tests raiding to the 999th power.

All test have `0.01` absolute tolerance for each element of resulting matrix.

## Submitting
When you are ready with task 1 or task 2: fork this repo, push your code and send the link to us.

Kosterov
