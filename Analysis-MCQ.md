# Multiple Choice Questions: Analysis of Parallel Algorithms

- **1. What is the definition of speedup in parallel computing?**

  - A) T(n, p) / T(n,1)
  - B) T(n,1) / T(n, p)
  - C) p \* T(n, p)
  - D) log(T(n, p))
  - **Correct Answer: B**

- **2. What is the maximum theoretical speedup on p processors according to Lemma 1?**

  - A) log(p)
  - B) p^2
  - C) p
  - D) n
  - **Correct Answer: C**

- **3. What is parallel efficiency defined as?**

  - A) T(n, p) / p
  - B) T(n,1) / (p \* T(n, p))
  - C) p / T(n, p)
  - D) log(p) / T(n,1)
  - **Correct Answer: B**

- **4. What is the serial runtime of matrix multiplication (assuming square matrices)?**

  - A) Θ(n log n)
  - B) Θ(n²)
  - C) Θ(n³)
  - D) Θ(n)
  - **Correct Answer: C**

- **5. According to Brent’s Lemma, if p2 < p1, what happens to efficiency?**

  - A) Efficiency is halved
  - B) Efficiency stays the same
  - C) Efficiency doubles
  - D) Efficiency becomes zero
  - **Correct Answer: B**

- **6. What does a work-efficient parallel algorithm aim for?**

  - A) Exponential speedup
  - B) Minimal number of processors
  - C) Constant-factor extra work compared to serial
  - D) Zero latency
  - **Correct Answer: C**

- **7. What is the formula for the parallel runtime of the sum operation?**

  - A) Θ(log n)
  - B) Θ(n/p + log p)
  - C) Θ(n²)
  - D) Θ(p log n)
  - **Correct Answer: B**

- **8. What is the optimal number of processors (p) to minimize runtime in parallel sum?**

  - A) log n
  - B) n
  - C) √n
  - D) n²
  - **Correct Answer: B**

- **9. What is the condition for parallel sum to maintain Θ(1) efficiency?**

  - A) p² = n
  - B) p log p = O(n)
  - C) log p = Θ(n)
  - D) p = Θ(n²)
  - **Correct Answer: B**

- **10. What can cause superlinear speedup in practice?**

  - A) Extra processors reduce accuracy
  - B) Cache effects improve performance
  - C) High memory latency
  - D) Processor collisions
  - **Correct Answer: B**

- **11. What is the formula for speedup when considering interconnect latency (τ)?**

  - A) S(n) ≈ T(n,1) / (n/p + log p)
  - B) S(p) ≈ n / (n/p + τ log p)
  - C) S(n) ≈ τ / log p
  - D) S(p) ≈ log n / τ
  - **Correct Answer: B**

- **12. What is the interconnect bandwidth defined as?**

  - A) Startup cost of transfer
  - B) Amount of parallel memory used
  - C) Average data transfer rate
  - D) Processor switching rate
  - **Correct Answer: C**

- **13. Which algorithm is preferred when the number of processors increases significantly?**

  - A) One with fixed time
  - B) One with higher p_max
  - C) One with fewer memory accesses
  - D) One with constant speedup
  - **Correct Answer: B**

- **14. In practice, what is the typical latency (τ) relative to computation?**

  - A) About equal
  - B) 10–100 times slower
  - C) 10^3–10^5 times slower
  - D) Negligible
  - **Correct Answer: C**

- **15. What is the total work in a parallel algorithm typically measured as?**
  - A) Memory usage
  - B) Processor-time product
  - C) Speedup per processor
  - D) Bandwidth per byte
  - **Correct Answer: B**
