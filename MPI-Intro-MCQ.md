# MPI Introduction

## Multiple Choice Questions

- **Question 1**: Which of the following best describes a process in the traditional sense according to the MPI documentation?

  - A) A thread with its own memory space
  - B) A program counter and address space
  - C) A program counter with multiple address spaces
  - D) A single program that runs on multiple data sets

  **Answer: B) A program counter and address space**

- **Question 2**: In the context of MPI, what does SPMD stand for?

  - A) Serial Programming for Multiple Devices
  - B) Simple Program, Multiple Datasets
  - C) Single Program, Multiple Data
  - D) Synchronized Parallel Memory Distribution

  **Answer: C) Single Program, Multiple Data**

- **Question 3**: What is a key advantage of the message-passing approach to communication as described in the document?

  - A) It requires only one process to explicitly participate
  - B) It decouples communication and synchronization
  - C) Any change in the receiving process's memory is made with the receiver's explicit participation
  - D) It allows for completely asynchronous operations

  **Answer: C) Any change in the receiving process's memory is made with the receiver's explicit participation**

- **Question 4**: What combination of elements forms a communicator in MPI?

  - A) A process and a tag
  - B) A group and a context
  - C) A datatype and a buffer
  - D) A rank and a size

  **Answer: B) A group and a context**

- **Question 5**: In MPI, which function would you use to identify which process you are in a parallel program?

  - A) MPI_Process_id
  - B) MPI_Comm_rank
  - C) MPI_Get_id
  - D) MPI_Process_rank

  **Answer: B) MPI_Comm_rank**

- **Question 6**: What is the purpose of tags in MPI message passing?

  - A) To identify different MPI implementations
  - B) To assist the receiving process in identifying the message
  - C) To specify the datatype of the message
  - D) To define the context of communication

  **Answer: B) To assist the receiving process in identifying the message**

- **Question 7**: When an MPI_SEND function returns, what can be said about the message?

  - A) The message has been received by the target process
  - B) The data has been delivered to the system and the buffer can be reused
  - C) The message is still in the local buffer and cannot be modified
  - D) The message has been copied to all processes in the communicator

  **Answer: B) The data has been delivered to the system and the buffer can be reused**

- **Question 8**: What happens if a process receives more data than specified by the count parameter in MPI_RECV?

  - A) The excess data is discarded
  - B) The receive operation continues until all data is received
  - C) It is considered an error
  - D) The excess data is stored in a system buffer for later retrieval

  **Answer: C) It is considered an error**

- **Question 9**: Why are datatypes important in MPI?

  - A) They are required only for backward compatibility
  - B) They allow communication between processes on machines with different memory representations
  - C) They are only used for error checking
  - D) They are needed only for collective operations

  **Answer: B) They allow communication between processes on machines with different memory representations**

- **Question 10**: What is the primary difference between contexts and tags in MPI?

  - A) Tags can use wildcards, contexts cannot
  - B) Contexts are for collective operations, tags are for point-to-point
  - C) Tags are system-defined, contexts are user-defined
  - D) Contexts are allocated at compile time, tags at runtime

  **Answer: A) Tags can use wildcards, contexts cannot**

- **Question 11**: What potential issue is demonstrated by the following code pattern?

  ```
  Process 0    Process 1
  Send(1)      Send(0)
  Recv(1)      Recv(0)
  ```

  - A) Race condition
  - B) Deadlock
  - C) Buffer overflow
  - D) Type mismatch

  **Answer: B) Deadlock**

- **Question 12**: Which two MPI collective operations can effectively replace SEND/RECEIVE in many numerical algorithms?

  - A) MPI_SCATTER and MPI_GATHER
  - B) MPI_BCAST and MPI_REDUCE
  - C) MPI_ALLTOALL and MPI_ALLGATHER
  - D) MPI_SCAN and MPI_EXSCAN

  **Answer: B) MPI_BCAST and MPI_REDUCE**

- **Question 13**: In a minimal MPI program, what is the correct order of core function calls?

  - A) MPI_Comm_rank, MPI_Init, program code, MPI_Finalize
  - B) MPI_Init, program code, MPI_Finalize, MPI_Comm_rank
  - C) MPI_Init, MPI_Comm_rank, program code, MPI_Finalize
  - D) Program code, MPI_Init, MPI_Comm_rank, MPI_Finalize

  **Answer: C) MPI_Init, MPI_Comm_rank, program code, MPI_Finalize**

- **Question 14**: What does MPI_COMM_WORLD represent?

  - A) A communicator created specifically for world-wide networks
  - B) The highest security level communicator available in MPI
  - C) The default communicator whose group contains all initial processes
  - D) A special communicator used only for collective operations

  **Answer: C) The default communicator whose group contains all initial processes**

- **Question 15**: Which of the following is NOT one of the basic six functions that many MPI programs can be written with?

  - A) MPI_INIT
  - B) MPI_COMM_SIZE
  - C) MPI_BARRIER
  - D) MPI_RECV

  **Answer: C) MPI_BARRIER**

## True/False Questions

- **Question 16**: MPI is a programming language specifically designed for parallel computing.

  **Answer: False** (MPI is a message-passing library specification, not a programming language)

- **Question 17**: In MPI, receiving fewer than the specified count of data items in MPI_RECV is considered an error.

  **Answer: False** (Receiving fewer items is acceptable, but receiving more is an error)

- **Question 18**: The function MPI_Reduce combines data from all processes in a communicator and returns it to one process.

  **Answer: True**

- **Question 19**: MPI can support communication between processes on machines with different memory representations.

  **Answer: True**

- **Question 20**: One-sided operations in MPI require both the sender and receiver to explicitly participate in the communication.

  **Answer: False** (One-sided operations require only one process to explicitly participate)
