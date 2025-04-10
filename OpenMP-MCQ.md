# OpenMP

## Multiple Choice Questions

- Which of the following best describes OpenMP's execution model?
  - A) Multiple independent processes running on separate memory spaces
  - B) A single process with multiple threads sharing the same memory
  - C) Master-slave architecture where the master distributes tasks to slaves
  - D) Client-server model where servers handle computation requests

Correct answer: B) A single process with multiple threads sharing the same memory

- What directive is used to create a parallel region in OpenMP?
  - A) #pragma omp for
  - B) #pragma omp parallel
  - C) #pragma omp section
  - D) #pragma omp create

Correct answer: B) #pragma omp parallel

- What happens when a variable is declared as "private" in an OpenMP parallel region?
  - A) A copy of the variable is created for each thread
  - B) All threads can only read the variable but not modify it
  - C) Only the master thread can access the variable
  - D) The variable can only be accessed in critical sections

Correct answer: A) A copy of the variable is created for each thread

- Which scheduling type in OpenMP automatically decreases chunk sizes as execution progresses?
  - A) static
  - B) dynamic
  - C) guided
  - D) auto

Correct answer: C) guided

- What is the purpose of the "reduction" clause in OpenMP?
  - A) To reduce the number of threads used in a parallel region
  - B) To combine partial results from threads using an associative operator
  - C) To decrease the memory usage of parallel regions
  - D) To optimize loop iterations by reducing computational complexity

Correct answer: B) To combine partial results from threads using an associative operator

- Which OpenMP construct ensures that only one thread executes a code block while others wait?
  - A) #pragma omp barrier
  - B) #pragma omp master
  - C) #pragma omp single
  - D) #pragma omp atomic

Correct answer: C) #pragma omp single

- What is the difference between #pragma omp single and #pragma omp master?
  - A) single allows any thread to execute the block, while master requires the master thread
  - B) single causes other threads to wait, while master does not
  - C) Both A and B
  - D) There is no difference between them

Correct answer: C) Both A and B

- Which of the following loop criteria is NOT supported by OpenMP parallel for directives?
  - A) Loop with a float iterator variable
  - B) Loop with unchanging boundary conditions
  - C) Loop with integer increments
  - D) Loop with comparison operators like < or <=

Correct answer: A) Loop with a float iterator variable

- What does the "schedule(static)" clause do in OpenMP?
  - A) Assigns iterations to threads at runtime based on availability
  - B) Divides iterations equally among threads before execution
  - C) Allows only one thread to execute at a time
  - D) Automatically adjusts the workload during execution

Correct answer: B) Divides iterations equally among threads before execution

- Which function would you use to get the ID of the current thread in OpenMP?
  - A) omp_get_thread_id()
  - B) omp_get_thread_num()
  - C) omp_thread_id()
  - D) omp_current_thread()

Correct answer: B) omp_get_thread_num()

- What synchronization mechanism ensures that memory operations are visible to all threads?
  - A) #pragma omp critical
  - B) #pragma omp barrier
  - C) #pragma omp flush
  - D) #pragma omp atomic

Correct answer: C) #pragma omp flush

- When using "firstprivate" in OpenMP, what happens to the variable?
  - A) A private copy is created for each thread with the initial value from the original variable
  - B) Only the first thread gets a private copy
  - C) The variable becomes read-only for all threads
  - D) The variable is initialized to zero for all threads

Correct answer: A) A private copy is created for each thread with the initial value from the original variable

- What is the primary challenge in parallelizing code with OpenMP?
  - A) Memory management
  - B) Race conditions and synchronization
  - C) CPU architecture limitations
  - D) Compiler support

Correct answer: B) Race conditions and synchronization

- What happens if OpenMP directives are compiled with a compiler that does not support OpenMP?
  - A) The code will not compile at all
  - B) The code will compile but crash at runtime
  - C) The directives are ignored and the code runs sequentially
  - D) The compiler automatically replaces directives with equivalent code

Correct answer: C) The directives are ignored and the code runs sequentially

- If multiple critical sections in different parts of the code use the same name, what happens?
  - A) They are mutually exclusive with each other
  - B) They can run concurrently with each other
  - C) The compiler will generate an error
  - D) The behavior is implementation-dependent

Correct answer: A) They are mutually exclusive with each other

## True/False Questions

- True or False: In OpenMP, global variables are private by default.

Correct answer: False (Global variables are shared by default)

- True or False: The "#pragma omp atomic" directive can protect any arbitrary code block as long as it's small.

Correct answer: False (It can only protect specific types of single variable updates)

- True or False: OpenMP allows for nested parallelism where parallel regions can contain other parallel regions.

Correct answer: True

- True or False: Using "#pragma omp ordered" guarantees that the specified block will be executed in the sequential order of iterations.

Correct answer: True

- True or False: The "schedule(dynamic)" option in OpenMP generally provides better load balancing than "schedule(static)" for irregular workloads.

Correct answer: True
