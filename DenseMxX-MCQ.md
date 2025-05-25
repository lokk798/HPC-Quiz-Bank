# MCQs on Dense Matrix Multiplication Algorithms

## 1. What is the main idea behind Cannon's algorithm?

- To rotate matrix blocks to align correctly for multiplication.
- To perform element-wise matrix addition.
- To avoid any data movement during computation.
- To compute determinants efficiently.
  **Answer:** - To rotate matrix blocks to align correctly for multiplication.

## 2. What kind of processor grid is required for Cannon’s algorithm?

- Linear
- Triangular
- Square 2D grid
- Hexagonal
  **Answer:** - Square 2D grid

## 3. What must be true about matrices A and B for Cannon’s algorithm?

- A must be symmetric
- B must be upper triangular
- Both must be square matrices
- They must be sparse
  **Answer:** - Both must be square matrices

## 4. What operation is central to SUMMA algorithm?

- Matrix transpose
- LU decomposition
- Outer product accumulation
- Inner product dotting
  **Answer:** - Outer product accumulation

## 5. What advantage does SUMMA have over Cannon’s algorithm?

- Requires triangular processor grid
- Handles sparse matrices only
- Works with non-square matrices and grids
- Avoids any form of broadcasting
  **Answer:** - Works with non-square matrices and grids

## 6. In SUMMA, what is broadcast within a processor row?

- Entire matrix B
- Column k of A
- Row k of B
- Diagonal of matrix A
  **Answer:** - Column k of A

## 7. What is broadcast within a processor column in SUMMA?

- Column k of A
- Row k of B
- The whole matrix C
- Diagonal of A
  **Answer:** - Row k of B

## 8. What happens after both row and column broadcasts in SUMMA?

- A transpose is taken
- Processors add A[i,k] \* B[k,j] to C[i,j]
- Matrices are rotated
- A new matrix is created
  **Answer:** - Processors add A[i,k] \* B[k,j] to C[i,j]

## 9. In SUMMA, what determines the number of outer loop iterations when using blocking?

- Number of rows
- Matrix diagonal size
- Block size `b`
- Number of processors
  **Answer:** - Block size `b`

## 10. In outer-product based matrix multiplication, which equation is correct?

- C = A × B + I
- C = ∑k A[:,k] × B[k,:]
- C = A · Bᵀ
- C = A ⊗ B
  **Answer:** - C = ∑k A[:,k] × B[k,:]

## 11. What is a core requirement for performing the outer-product version of matrix multiplication?

- A must be diagonal
- Inner dimension must match
- Matrix must be identity
- No broadcasting should be involved
  **Answer:** - Inner dimension must match

## 12. What is a drawback of Cannon’s algorithm?

- Works only on single processors
- Requires sparse matrices
- Requires square 2D processor grids
- Cannot handle blocking
  **Answer:** - Requires square 2D processor grids

## 13. Which type of multiplication does inner-product method compute?

- A[:,i] × B[i,:]
- A[i,:] · B[:,j]
- A ⊗ B
- A \* Bᵀ
  **Answer:** - A[i,:] · B[:,j]

## 14. Which of these is a key benefit of SUMMA?

- Zero communication overhead
- Avoids need for square matrices or grids
- Handles only symmetric matrices
- Requires matrix pre-alignment
  **Answer:** - Avoids need for square matrices or grids

## 15. What is the total communication cost in SUMMA with optimal block size?

- O(n³)
- O(p²)
- O((τ + μn²/p)(log p))
- O(n)
  **Answer:** - O((τ + μn²/p)(log p))
