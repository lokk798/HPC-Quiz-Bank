# Multiple Choice Questions on Ray Framework

- **1. When was Ray initially started as a class project?**  
  A. 2017  
  B. 2016  
  C. 2015  
  D. 2018  
  **Answer:** B

- **2. What was the primary goal of Ray at the beginning?**  
  A. Distributed database management  
  B. Accelerating classic machine learning  
  C. Scaling distributed deep learning and reinforcement learning  
  D. Cloud infrastructure orchestration  
  **Answer:** C

- **3. Which library was released in 2017 alongside Ray Tune?**  
  A. Ray Data  
  B. RLlib  
  C. Ray Serve  
  D. Ray Core  
  **Answer:** B

- **4. What does the `@ray.remote` decorator indicate?**  
  A. Run synchronously  
  B. Mark a class or function for remote execution  
  C. Automatically log errors  
  D. Compress function output  
  **Answer:** B

- **5. What type of system is Ray designed to unify?**  
  A. Web applications  
  B. Distributed computing workloads  
  C. Mobile platforms  
  D. Blockchain nodes  
  **Answer:** B

- **6. What is used in Ray to refer to a potentially not-yet-created object?**  
  A. Promise  
  B. Reference  
  C. Future  
  D. Proxy  
  **Answer:** C

- **7. What is the main advantage of using actors in Ray?**  
  A. Stateless operation  
  B. Enhanced debuggability  
  C. Support for complex stateful operations  
  D. Faster I/O operations  
  **Answer:** C

- **8. What is the purpose of `ray.put()`?**  
  A. Execute a task remotely  
  B. Schedule a function  
  C. Store an object and get its ID  
  D. Fetch result from a remote function  
  **Answer:** C

- **9. What scheduling improvement was made for actor method invocations?**  
  A. Shared control plane  
  B. Linear resource allocation  
  C. Direct actor calls bypassing the scheduler  
  D. Hierarchical scheduling tree  
  **Answer:** C

- **10. What does Ray use to support low-overhead GPU-GPU transfers in compiled graphs?**  
  A. Shared CPU memory  
  B. RDMA  
  C. TorchTensorType with NCCL transport  
  D. JSON communication  
  **Answer:** C

- **11. What feature allows tasks to be scheduled based on ephemeral, logical resources?**  
  A. Cloud quotas  
  B. Virtual CPUs  
  C. Ephemeral resources  
  D. Static priorities  
  **Answer:** C

- **12. What is a key benefit of Ray’s compiled graphs?**  
  A. Eliminate the need for Python  
  B. Support for multi-node training  
  C. Reduced control RPCs and static resource reuse  
  D. Real-time garbage collection  
  **Answer:** C

- **13. Which of the following is NOT a challenge Ray aimed to address?**  
  A. Homogeneous cluster optimization  
  B. Complex AI pipelines  
  C. GPU-accelerated training  
  D. Distributed model serving  
  **Answer:** A

- **14. How does Ray achieve fault tolerance for lost objects?**  
  A. Persistent disk logging  
  B. Retry mechanisms in the driver  
  C. Lineage-based object reconstruction  
  D. Stateful snapshot backups  
  **Answer:** C

- **15. What motivated Ray’s transition from task-only abstraction to also include actors?**  
  A. To support UI rendering  
  B. For improved code readability  
  C. To handle stateful computations and improve GPU performance  
  D. Reduce memory usage  
  **Answer:** C
