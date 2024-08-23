# Array

## Definition

Contiguous area of memory consisting of equal-size elements indexed by contiguous integers.

## Indexing

Indexing of arrays can vary between languages commonly used is the 0 based index, but some languages use 1 based indexing or lets the user decide the starting index.

## Constant-time access

The most important feature of an array is the constant-time and random access it grants.
The compiler accesses an array by using a simple [arithmetic](to be added) algorithm

```Java
array_addr + elem_size * (i - first_index)
```

array_addr: this is the address where the array is stored
elem_size: size of the array
i: the index we want to access
first_index: the first index of the array, only needed if we do not use 0 based indexing

## Multi-Dimensional Arrays

A multi-dimensional array can be termed as an array of arrays that stores homogeneous data in tabular form.

Accessing the data of a multi-dimensional array can also be done by using [arithmetics](to be added)
Example for an 3 x 6 (rows x columns) dimensional array

```Java
array_addr + elem_size * ((row_index - first_row_index) * row_elem_size + (col_index - first_col_index))
```

row_index: the index of the row we want to access
first_row_index: the first index of the rows, only needed if we do not use 0 based indexing
row_elem_size: the amount of columns a row contains
col_index: the index of the column we want to access
first_col_index: the first index of the columns, only needed if we do not use 0 based indexing

### Ordering/Indexing

Row-major ordering/indexing means the array is laid out by ascending row index:
(1, 1), (1, 2), (1, 3), (2, 1) (2, 2), (2, 3), (3, 1), (3, 2), (3, 3)

Column-major ordering/indexing means the array is laid out by ascending column index:
(1, 1), (2, 1), (3, 1), (1, 2), (2, 2), (3, 2), (1, 3), (2, 3), (3, 3)

## Performance of common Operations

|           | Add  | Remove |
| --------- | ---- | ------ |
| Beginning | O(n) |  O(n)  |
| End       | O(1) |  O(1)  |
| Arbitrary | O(n) |  O(n)  |

## Source

---

Course: <https://www.coursera.org/lecture/data-structures/arrays-OsBSF>
Other: <https://www.geeksforgeeks.org/multidimensional-arrays-in-c/>
---
