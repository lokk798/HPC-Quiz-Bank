# Parallel Programming Design Patterns

## Multiple Choice Questions

- Which of the following is NOT an example of an "Embarrassingly Parallel" computation?

  - A) Vector sum
  - B) Mandelbrot set calculation
  - C) Five-point stencil computation
  - D) Brute force password cracking
  - Answer: C) Five-point stencil computation

- In the context of parallel programming patterns, what is the primary characteristic of the "Partition" pattern?

  - A) The input data is partitioned among processors with no communication needed
  - B) The input data space is split into disjoint regions, and each processor operates on one partition
  - C) A master process distributes tasks to worker processes dynamically
  - D) All processors perform the same operation on different data elements
  - Answer: B) The input data space is split into disjoint regions, and each processor operates on one partition

- What is the primary concern when choosing the optimal partition size in parallel programming?

  - A) The number of available processors
  - B) The type of computation being performed
  - C) Balancing scheduling overhead against workload imbalance
  - D) Minimizing memory usage
  - Answer: C) Balancing scheduling overhead against workload imbalance

- When implementing stencil computations on distributed-memory architectures, what technique is essential for efficiency?

  - A) Dynamic task allocation
  - B) Ghost cells
  - C) Cyclic partitioning
  - D) Scan operations
  - Answer: B) Ghost cells

- What is the time complexity for performing a reduction operation in parallel?

  - A) O(n)
  - B) O(log n)
  - C) O(n log n)
  - D) O(1)
  - Answer: B) O(log n)

- In the context of partitioning, what does "fine-grained" partitioning refer to?

  - A) A partition with small number of large blocks
  - B) A partition with large number of small blocks
  - C) A partition with irregular shapes
  - D) A partition with regular shapes
  - Answer: B) A partition with large number of small blocks

- Which pattern is most effective for handling uneven workload distribution?

  - A) Embarrassingly Parallel
  - B) Stencil
  - C) Master-Worker
  - D) Scan
  - Answer: C) Master-Worker

- What is the primary difference between inclusive-scan and exclusive-scan operations?

  - A) Inclusive-scan includes the current element, while exclusive-scan does not
  - B) Inclusive-scan works only with addition, while exclusive-scan works with any binary operator
  - C) Inclusive-scan is parallelizable, while exclusive-scan is not
  - D) Inclusive-scan works on arrays, while exclusive-scan works on matrices
  - Answer: A) Inclusive-scan includes the current element, while exclusive-scan does not

- For the Line of Sight problem, which parallel programming pattern is used to compute the maximum slopes seen so far?

  - A) Reduce
  - B) Scan
  - C) Stencil
  - D) Partition
  - Answer: B) Scan

- Which of the following statements about the "work efficiency" of the tree-structured reduction algorithm is true?

  - A) It performs more operations than the optimal serial algorithm
  - B) It performs fewer operations than the optimal serial algorithm
  - C) It performs the same number of operations as the optimal serial algorithm
  - D) Its efficiency depends on the specific operator being used
  - Answer: C) It performs the same number of operations as the optimal serial algorithm

- In the 2D Block Partitioning of a matrix, what does "Block, Block" partitioning mean?

  - A) The matrix is partitioned into blocks along both dimensions
  - B) The matrix is partitioned into blocks only along the rows
  - C) The matrix is partitioned into blocks only along the columns
  - D) The matrix is not partitioned
  - Answer: A) The matrix is partitioned into blocks along both dimensions

- What is the main issue with using a regular partitioning for the Mandelbrot set calculation?

  - A) Memory requirements are too high
  - B) Uneven load distribution due to varying computational complexity across the domain
  - C) The algorithm is inherently sequential
  - D) The resolution of the result is compromised
  - Answer: B) Uneven load distribution due to varying computational complexity across the domain

- What is the primary purpose of ghost cells in stencil computations?

  - A) To reduce memory usage
  - B) To handle boundary conditions
  - C) To improve cache performance
  - D) To facilitate dynamic load balancing
  - Answer: B) To handle boundary conditions

- What is Christopher Alexander known for in the context of design patterns?

  - A) Inventing the Master-Worker paradigm
  - B) Developing the first parallel computing architecture
  - C) First using the term "architectural pattern" in building design
  - D) Creating the stencil computation pattern
  - Answer: C) First using the term "architectural pattern" in building design

- What type of stencil represents the Moore neighborhood in 2D?
  - A) 5-point 2-axis stencil
  - B) 7-point 3-axis stencil
  - C) 9-point 1-plane stencil
  - D) 13-point 3-axis stencil
  - Answer: C) 9-point 1-plane stencil

## True/False Questions

- True or False: In the Master-Worker paradigm, the number of tasks should ideally be equal to the number of available processors.

  - Answer: False (The number of tasks should be significantly larger than the number of processors for effective load balancing)

- True or False: A reduction operation requires O(n) parallel steps with n processors.

  - Answer: False (It requires O(log n) parallel steps)

- True or False: Block partitioning and cyclic partitioning will always result in the same load balance for any computation.

  - Answer: False (Different partitioning strategies can result in different load balances depending on the computation)

- True or False: The scan operation can be implemented efficiently in parallel with a work-efficient algorithm.

  - Answer: True

- True or False: In stencil computations, two domains (current and next) are typically used to avoid overwriting values needed for subsequent calculations.
  - Answer: True
