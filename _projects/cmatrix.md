---
layout: default
title: C++ Matrix Library - cmatrix
---

## {{ page.title }}

[GitHub](https://github.com/benapier/cmatrix)

A simple matrix library in C++ which takes advantage of operator overloading so that matrices can be treated like any other common data types (double, integer, etc.).

Current features:
* Basic matrix arithmetic (addition, subtraction, multiplication)
* Basic scalar arithmetic (multiplication, division)
* Transposition
* Determinants
* Inverse

Planned features:
* Concatination
* Kronecker multiplication
* Hadanard multiplication

### Example

Find values for *x*, *y*, and *z* that satisfy:

<img src="/../assets/cmatrix_problem.svg" width="150" />

```c++
// Entering in the values in a matrix
mat mat_a = mat(3, 3);
mat_a(0, 0) = 3;
mat_a(0, 1) = 4;
// ...
mat(2, 1) = 3;
mat(2, 2) = -2;

mat mat_b = mat(3, 1);
mat_b(0, 0) = 3;
mat_b(1, 0) = 6;
mat_b(2, 0) = 11;

mat answer = mat_a.inverse() * mat_b;
double x, y, z;
x = answer(0, 0);
y = answer(1, 0);
z = answer(2, 0);
```

