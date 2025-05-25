# Parallel Sorting Algorithms - MCQ

- **1. What is the best possible time complexity achievable using parallel sorting with `n` processing units for comparison-based algorithms?**  
  A. O(n)  
  B. O(log(n)) ✅  
  C. O(n log(n))  
  D. O(n²)

- **2. What operation is central to many parallel sorting algorithms?**  
  A. Divide-and-conquer  
  B. Binary search  
  C. Compare-and-exchange ✅  
  D. Hashing

- **3. In the first version of parallel compare-and-exchange, what happens?**  
  A. Each processor performs its own compare  
  B. P1 sends A to P2, which sends back min(A, B) ✅  
  C. Both processors exchange values simultaneously  
  D. No communication occurs

- **4. Which sorting algorithm naturally benefits from a pipeline implementation in parallel?**  
  A. Quicksort  
  B. Bubble Sort ✅  
  C. Insertion Sort  
  D. Selection Sort

- **5. What is the time complexity of the sequential bubble sort algorithm?**  
  A. O(n log(n))  
  B. O(n)  
  C. O(n²) ✅  
  D. O(log(n))

- **6. Odd-even transposition sort alternates between which two phases?**  
  A. Split and Merge  
  B. Sort and Compare  
  C. Even and Odd ✅  
  D. Merge and Partition

- **7. What is the time complexity of parallel odd-even transposition sort?**  
  A. O(log(n))  
  B. O(n²)  
  C. O(n) ✅  
  D. O(n log(n))

- **8. What does parallel mergesort primarily take advantage of?**  
  A. Random pivots  
  B. Balanced binary trees  
  C. The tree structure of merge operations ✅  
  D. Bubble comparisons

- **9. What is the average time complexity of Quicksort?**  
  A. O(n²)  
  B. O(n log(n)) ✅  
  C. O(log(n))  
  D. O(n)

- **10. In parallel quicksort, what affects load balancing and efficiency?**  
  A. Number of threads  
  B. Pivot selection ✅  
  C. Use of GPUs  
  D. Cache size

- **11. How many compare-and-exchange operations are required in odd-even merge for two lists of size `n`?**  
  A. n  
  B. n/2  
  C. n − 1 ✅  
  D. 2n

- **12. What is the time complexity of the parallel odd-even merge sort?**  
  A. O(n log(n))  
  B. O(log(n))  
  C. O(log(n)²) ✅  
  D. O(n²)

- **13. What type of sequence is a prerequisite for applying bitonic mergesort?**  
  A. Increasing only  
  B. Bitonic ✅  
  C. Random  
  D. Uniform

- **14. What is the total number of steps needed in parallel bitonic mergesort for list size `n = 2^k`?**  
  A. log(n)  
  B. k(k + 1)/2 ✅  
  C. n log(n)  
  D. n/2

- **15. According to the time complexity summary, which two parallel algorithms have complexity O(log(n)²)?**  
  A. Bubble sort and mergesort  
  B. Quicksort and mergesort  
  C. Odd-even mergesort and bitonic mergesort ✅  
  D. Quicksort and bubble sort
