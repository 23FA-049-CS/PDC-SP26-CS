```
# Chapter 3 – Process Based Parallelism in Python
```

```
---
```

```
## Topic: Communication with Pipe
```

```
**What I Learned**
```

```
I learned how two processes communicate using pipes. One process sends data and
the other receives and processes it.
```

```
**How to Execute**
```

```
python pipe.py
```

```
**Use / Output**
```

```
One process sends numbers from 0 to 9 and another process receives them and
squares them.
```

```
**When to Use**
```

```
When two processes need direct communication.
```

```
**Advantages**
```

- `Fast communication between processes` 

- `Useful for real-time data transfer` 

```
**Disadvantages**
```

- `Complex implementation` 

- `Hard to debug` 

```
**Summary**
```

```
Pipe allows direct communication between two processes.
```

```
---
```

## `## Topic: Communication with Queue` 

```
**What I Learned**
```

```
I learned how processes share data safely using a queue.
```

```
**How to Execute**
python queue.py
```

```
**Use / Output**
Producer adds items and consumer removes items from queue.
```

```
**When to Use**
When multiple processes need safe communication.
```

```
**Advantages**
- Safe for multiple processes
```

- `Easy implementation` 

- `**Disadvantages** - Can be slow for large data` 

```
**Summary**
Queue is used for safe inter-process communication.
```

```
---
```

```
## Topic: Killing Processes
```

```
**What I Learned**
I learned how to stop a running process using terminate method.
```

```
**How to Execute**
python terminate.py
**Use / Output**
Process starts and is then forcefully stopped.
```

```
**When to Use**
When a process is not responding or is no longer needed.
**Advantages**
- Gives control over processes
**Disadvantages**
- May cause data loss
- Unsafe termination
```

```
**Summary**
Processes can be stopped using terminate method.
```

```
---
```

```
## Topic: Function in Process
```

```
**What I Learned**
I learned how functions run inside processes.
**How to Execute**
Used inside multiprocessing process execution.
**Use / Output**
Function prints numbers from 0 to i.
```

```
**When to Use**
When simple function-based execution is needed.
```

```
**Advantages**
- Simple implementation
**Disadvantages**
- No advanced control
```

```
**Summary**
Functions can be executed inside processes.
```

```
---
```

```
## Topic: Naming Processes
**What I Learned**
I learned how to assign names to processes.
**How to Execute**
python naming.py
**Use / Output**
Processes display their names during execution.
```

```
**When to Use**
For debugging and tracking processes.
```

```
**Advantages**
- Easy identification
```

- `Helpful in debugging` 

```
**Disadvantages**
- No functional effect
**Summary**
Naming helps identify processes.
---
```

```
## Topic: Process Subclass
**What I Learned**
I learned how to create processes using class inheritance.
**How to Execute**
python subclass.py
**Use / Output**
Multiple custom processes are executed.
**When to Use**
When custom behavior is required.
**Advantages**
- Reusable structure
- Organized code
**Disadvantages**
- Slightly complex
**Summary**
Processes can be created using subclassing.
```

```
---
```

```
## Topic: Process Pool
```

```
**What I Learned**
I learned how to use process pools for parallel execution.
**How to Execute**
python pool.py
**Use / Output**
Squares numbers from 0 to 99 using multiple processes.
**When to Use**
For large batch processing tasks.
**Advantages**
- Efficient CPU usage
- Faster execution
**Disadvantages**
- Higher memory usage
**Summary**
Process pool runs tasks in parallel.
```

```
## Topic: Process Barrier
```

```
**What I Learned**
I learned how processes synchronize using a barrier.
```

```
**How to Execute**
python barrier.py
**Use / Output**
Processes wait until all reach the same point before continuing.
```

```
**When to Use**
When synchronization is required.
```

```
**Advantages**
- Ensures coordination
```

```
**Disadvantages**
- One slow process delays all
**Summary**
Barrier synchronizes processes.
```

```
## Topic: Background Process
```

```
**What I Learned**
I learned difference between daemon and normal process.
**How to Execute**
python background.py
**Use / Output**
Daemon process runs in background and stops when main program ends.
**When to Use**
For background tasks.
```

```
**Advantages**
- Runs in background
```

- `Does not block main program` 

```
**Disadvantages**
- Cannot be controlled easily
**Summary**
Daemon processes run in background.
```

```
## Topic: Spawning Processes
```

```
**What I Learned**
I learned how to create multiple processes dynamically.
**How to Execute**
python spawning.py
**Use / Output**
Multiple processes execute same function.
**When to Use**
For parallel execution.
**Advantages**
- Fast execution
- Uses multiple CPU cores
```

```
**Disadvantages**
```

```
- Hard to manage many processes
```

```
**Summary**
Spawning creates multiple processes.
```

```
## Topic: Spawning with Namespace
```

```
**What I Learned**
```

```
I learned how to use external functions inside processes.
```

```
**How to Execute**
python namespace.py
```

```
**Use / Output**
Processes execute imported function.
```

```
**When to Use**
When code is modular.
```

```
**Advantages**
```

- `Code reuse` 

- `Clean structure` 

```
**Disadvantages**
```

- `Dependency issues possible` 

```
**Summary**
External functions can be used in processes.
```

