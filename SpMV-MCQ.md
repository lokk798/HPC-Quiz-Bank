# Sparse Matrix-Vector Multiplication (SpMV) - MCQs

### 1. What defines a sparse matrix?

- A matrix with negative entries
- A matrix with primarily non-zero values
- A matrix with > 90% zeros (✓)
- A matrix that changes size dynamically

### 2. Why is it inefficient to use dense structures for sparse matrices?

- They require more code
- They are slower to access
- They waste memory and computation (✓)
- They are hard to parallelize

### 3. Which of the following is NOT an application of sparse matrices?

- Simulating climate
- Analyzing images
- Solving Sudoku (✓)
- Page ranking

### 4. What is the primary benefit of the CSR format?

- Reduces matrix dimensions
- Makes diagonal entries more accessible
- Cache-efficient storage and traversal (✓)
- Makes the matrix symmetric

### 5. Which of these is NOT a common sparse matrix format?

- CSR
- CSC
- DIAG
- PDF (✓)

### 6. In CSR format, what does the `ptr` array store?

- Column indices of non-zero elements
- Row start pointers (✓)
- Non-zero values
- Diagonal values

### 7. What is stored in the `val` array in CSR format?

- Row indices
- Column indices
- Non-zero values (✓)
- Number of zeros in each row

### 8. What kind of matrices often represent undirected graphs?

- Symmetric matrices (✓)
- Identity matrices
- Dense matrices
- Diagonal matrices

### 9. Which array in CSR format holds the column indices of non-zero elements?

- ptr
- val
- ind (✓)
- col

### 10. What is the time complexity of SpMV for a matrix with `nnz` non-zero elements?

- O(n²)
- O(nnz) (✓)
- O(1)
- O(log n)

### 11. What does the COO format store for each non-zero element?

- Only its value
- Row and column indices
- Row, column, and value (✓)
- Row and value only

### 12. Why is the diagonal format useful in GPU computing?

- It minimizes branching
- It avoids random memory access (✓)
- It stores only upper triangle
- It compresses more than CSR

### 13. In parallel SpMV using CSR, which data structure is reused the most?

- A matrix entries
- y vector entries (✓)
- x vector entries
- None of the above

### 14. What is the segmented scan technique used for?

- Converting dense to sparse matrices
- Reversing a sparse matrix
- Efficient parallel SpMV accumulation (✓)
- Sorting matrix rows

### 15. Which format stores blocks of small dense submatrices?

- Diagonal
- CSC
- Blocked (✓)
- Symmetric
