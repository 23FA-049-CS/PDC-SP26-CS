```
# Chapter 4 – MPI (Message Passing Interface) in Python
```

```
---
```

```
## Topic: Alltoall Communication
```

```
**What I Learned**
```

```
I learned how each process sends and receives data from all other processes
using Alltoall communication.
```

```
**How to Execute**
```

```
mpiexec -n 4 python alltoall.py
```

```
**Use / Output**
```

```
Each process sends data to all other processes and receives data from them.
```

```
**When to Use**
When full communication between all processes is required.
```

```
**Advantages**
```

- `Full data exchange between processes` 

- `Useful in parallel matrix operations` 

```
**Disadvantages**
```

- `High communication cost` 

- `Not scalable for large systems` 

```
**Summary**
Alltoall is used for complete data exchange between processes.
```

```
---
```

```
## Topic: Broadcast
```

```
**What I Learned**
```

```
I learned how one process shares data with all other processes.
```

```
**How to Execute**
mpiexec -n 4 python broadcast.py
```

```
**Use / Output**
Root process sends a variable to all other processes.
```

```
**When to Use**
When same data is needed by all processes.
```

```
**Advantages**
```

```
- Simple data sharing
```

- `Efficient for common values` 

- `**Disadvantages** - Only one source of data` 

```
**Summary**
Broadcast sends data from one process to all processes.
```

```
---
```

```
## Topic: Deadlock Problem
```

```
**What I Learned**
```

```
I learned how deadlock occurs when two processes wait for each other to
send/receive data.
```

```
**How to Execute**
mpiexec -n 6 python deadlock.py
**Use / Output**
Processes 1 and 5 wait on each other causing blocking behavior.
```

```
**When to Use**
Used for understanding synchronization problems.
```

```
**Advantages**
- Helps understand MPI synchronization issues
```

```
**Disadvantages**
- Causes program freeze
```

```
- Poor design leads to deadlock
```

```
**Summary**
Deadlock happens when processes wait indefinitely for each other.
```

```
---
```

```
## Topic: Gather
**What I Learned**
I learned how multiple processes send data to one root process.
**How to Execute**
mpiexec -n 4 python gather.py
**Use / Output**
All processes send computed values to root process.
```

```
**When to Use**
When collecting data from multiple processes.
```

```
**Advantages**
- Centralized data collection
- Easy aggregation
```

```
**Disadvantages**
- Root process overload
```

```
**Summary**
Gather collects data from all processes to root.
```

```
---
```

```
## Topic: Hello World MPI
```

```
**What I Learned**
```

```
I learned how MPI processes are initialized and how each process has a unique
rank.
```

```
**How to Execute**
mpiexec -n 4 python helloworld.py
```

```
**Use / Output**
Each process prints its rank.
```

```
**When to Use**
To test MPI setup.
```

```
**Advantages**
- Simple verification program
```

```
**Disadvantages**
- No practical computation
```

```
**Summary**
Each MPI process runs independently and has a rank.
```

```
---
```

```
## Topic: Point to Point Communication
```

```
**What I Learned**
I learned how processes directly send and receive messages.
```

```
**How to Execute**
mpiexec -n 9 python send_recv.py
**Use / Output**
Processes send messages to specific target processes.
```

```
**When to Use**
When direct communication is needed.
```

```
**Advantages**
- Precise communication
```

- `Efficient for small data exchange` 

- `**Disadvantages** - Requires correct process coordination` 

```
**Summary**
Point-to-point communication sends data between specific processes.
```

```
---
```

```
## Topic: Reduction
```

```
**What I Learned**
I learned how to combine data from all processes using a reduction operation.
```

```
**How to Execute**
mpiexec -n 4 python reduce.py
**Use / Output**
All process data is summed and sent to root.
```

```
**When to Use**
When performing aggregation operations.
```

```
**Advantages**
- Efficient computation
```

```
- Useful for mathematical operations
```

```
**Disadvantages**
- Only root gets final result
```

```
**Summary**
Reduce combines data from all processes.
```

```
---
```

```
## Topic: Scatter
```

```
**What I Learned**
```

```
I learned how root process distributes data to all processes.
```

```
**How to Execute**
mpiexec -n 4 python scatter.py
```

```
**Use / Output**
Array is split and distributed among processes.
```

```
**When to Use**
When distributing tasks.
```

```
**Advantages**
```

- `Balanced workload distribution` 

- `**Disadvantages** - Requires proper data size` 

```
**Summary**
Scatter distributes data from root to all processes.
```

```
---
```

```
## Topic: Virtual Topology
```

```
**What I Learned**
```

```
I learned how processes can be arranged in a grid using Cartesian topology.
```

```
**How to Execute**
mpiexec -n 4 python virtualtopology.py
```

```
**Use / Output**
Processes are assigned neighbors in UP, DOWN, LEFT, RIGHT directions.
```

```
**When to Use**
In grid-based simulations like matrix or image processing.
```

```
**Advantages**
```

- `Structured communication` 

- `Easy neighbor identification` 

```
**Disadvantages**
```

- `Complex setup` 

```
**Summary**
```

```
Virtual topology organizes processes in a grid structure.
```

