# CUDA Basics

## Multiple Choice Questions

- Which of the following CUDA keywords indicates that a function runs on the GPU and is called from the host?
  - A) **device**
  - B) **global**
  - C) **host**
  - D) **kernel**
- Correct answer: B) **global**

- In CUDA programming, what does the triple angle bracket notation (<<<...>>>) specify?
  - A) The memory space to be used
  - B) The number of threads and blocks to launch
  - C) The type of operation to perform
  - D) The synchronization mode
- Correct answer: B) The number of threads and blocks to launch

- What is the correct way to allocate memory on the GPU in CUDA?
  - A) malloc()
  - B) new
  - C) cudaMalloc()
  - D) gpuAlloc()
- Correct answer: C) cudaMalloc()

- Which variable is used to access the thread index within a block?
  - A) threadId.x
  - B) threadNum.x
  - C) threadIdx.x
  - D) thread.x
- Correct answer: C) threadIdx.x

- How do threads within the same block communicate with each other in CUDA?
  - A) Through global memory
  - B) Through shared memory
  - C) Through constant memory
  - D) Through texture memory
- Correct answer: B) Through shared memory

- What is the purpose of the \_\_syncthreads() function in CUDA?
  - A) To synchronize the CPU and GPU execution
  - B) To synchronize all threads across different blocks
  - C) To synchronize all threads within a block
  - D) To terminate thread execution
- Correct answer: C) To synchronize all threads within a block

- What is the correct formula to calculate a unique global index for a thread in a 1D grid with multiple blocks?
  - A) blockIdx.x + threadIdx.x
  - B) threadIdx.x \* blockIdx.x
  - C) threadIdx.x + blockIdx.x \* blockDim.x
  - D) blockIdx.x + threadIdx.x \* gridDim.x
- Correct answer: C) threadIdx.x + blockIdx.x \* blockDim.x

- Which memory copy function blocks the CPU until the copy operation is complete?
  - A) cudaMemcpy()
  - B) cudaMemcpyAsync()
  - C) cudaBlockingCopy()
  - D) cudaSyncCopy()
- Correct answer: A) cudaMemcpy()

- In CUDA, the host refers to:
  - A) The GPU and its memory
  - B) The CPU and its memory
  - C) The shared memory
  - D) The block of threads
- Correct answer: B) The CPU and its memory

- Which of the following is true about kernel launches in CUDA?
  - A) They are synchronous and block the CPU
  - B) They are asynchronous and do not block the CPU
  - C) They must be followed by a cudaMemcpy() call
  - D) They can only launch one block at a time
- Correct answer: B) They are asynchronous and do not block the CPU

- What does the compute capability of a CUDA device describe?
  - A) The maximum number of concurrent threads
  - B) The architecture, features, and capabilities of the device
  - C) The clock speed of the GPU
  - D) The amount of global memory available
- Correct answer: B) The architecture, features, and capabilities of the device

- Which function would you use to get information about the last CUDA error that occurred?
  - A) cudaGetError()
  - B) cudaLastError()
  - C) cudaGetLastError()
  - D) cudaCheckError()
- Correct answer: C) cudaGetLastError()

- What is the primary purpose of shared memory in CUDA?
  - A) To store constant values that don't change during kernel execution
  - B) To enable fast communication and data sharing between threads in a block
  - C) To transfer data between the host and device
  - D) To store the program code that runs on the GPU
- Correct answer: B) To enable fast communication and data sharing between threads in a block

- When implementing a stencil operation in CUDA, why is \_\_syncthreads() necessary?
  - A) To ensure all threads have completed writing to global memory
  - B) To prevent the CPU from continuing execution before the GPU
  - C) To prevent data hazards when threads read shared memory values written by other threads
  - D) To optimize memory bandwidth
- Correct answer: C) To prevent data hazards when threads read shared memory values written by other threads

- Which of the following accurately describes the relationship between blocks and threads in CUDA?
  - A) A block contains multiple threads that can communicate via shared memory
  - B) A thread contains multiple blocks that can communicate via global memory
  - C) Blocks and threads are synonymous terms in CUDA
  - D) A grid contains multiple threads which are grouped into blocks
- Correct answer: A) A block contains multiple threads that can communicate via shared memory

## True/False Questions

- True or False: In CUDA, device pointers can be dereferenced in host code.
- Correct answer: False

- True or False: The cudaDeviceSynchronize() function blocks the CPU until all preceding CUDA calls have completed.
- Correct answer: True

- True or False: Each CUDA thread can access the shared memory of any block in the grid.
- Correct answer: False

- True or False: The blockDim built-in variable refers to the dimensions of the grid in a CUDA kernel.
- Correct answer: False (It refers to the dimensions of the block)

- True or False: CUDA textures provide hardware acceleration for linear and bilinear filtering operations.
- Correct answer: True
