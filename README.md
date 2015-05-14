# ndarray-lup-factorization-2

LU factorization with pivoting for ndarrays

# Introduction

This module performs an in-place LUP factorization (LU with partial pivoting) on matrix A. Be advised that the rows are physically swapped which is slightly sub-optimal.

The resulting factorization is PA = LU where P is a permutation matrix.

For an alternate version, see: [ndarray-lup-factorization](https://github.com/scijs/ndarray-lup-factorization)

# Usage

##### require('ndarray-lup-factorization-2')( A, L, P )

Inputs:
- A: An n x n ndarray. This matrix is overwritten during the factorization. At the end of the factorization, the upper-triangular portion contains U and the lower-triangular portion contains zeros.
- L: An n x n ndarray. At the end of the factorization, this array contains the lower-triangular portion of the factorization.
- P: An `Array`. At the end of the factorization, this contains a vector representation of the permutation matrix. The P[i]th element of the ith row of the permutation matrix is one; all others elements are zero.