```
# Chapter 5 – Asyncio and Concurrent Futures in Python
```

```
---
```

```
## Topic: Asyncio and Future
```

```
**What I Learned**
```

```
I learned how asyncio uses futures and coroutines to run tasks asynchronously
and return results later.
```

```
**How to Execute**
```

```
python async_future.py num1 num2
```

```
**Use / Output**
```

```
One coroutine calculates sum of numbers and another calculates factorial, both
run asynchronously and return results.
```

```
**When to Use**
```

```
When multiple independent tasks need to run concurrently.
```

```
**Advantages**
```

```
- Non-blocking execution
```

- `Efficient for I/O tasks` 

```
**Disadvantages**
```

- `Complex flow control` 

- `Hard to debug` 

```
**Summary**
Futures allow asynchronous execution and result handling in asyncio.
```

```
---
```

```
## Topic: Asyncio Coroutine
```

```
**What I Learned**
```

```
I learned how coroutines can be used to create a finite state machine using
asyncio.
```

```
**How to Execute**
python state_machine.py
```

```
**Use / Output**
Program switches between different states based on random values.
```

```
**When to Use**
For simulations and state-based systems.
```

```
**Advantages**
- Efficient asynchronous transitions
```

```
- Good for simulations
```

```
**Disadvantages**
- Hard to understand flow
```

- `Debugging complexity` 

```
**Summary**
Coroutines can simulate state machines using async flow.
```

```
---
```

```
## Topic: Asyncio Event Loop
```

```
**What I Learned**
```

```
I learned how event loop schedules and runs multiple tasks over time.
```

```
**How to Execute**
python event_loop.py
**Use / Output**
Tasks A, B, and C run repeatedly in sequence using loop scheduling.
```

```
**When to Use**
When tasks need timed execution.
```

```
**Advantages**
- Controlled scheduling
- Efficient task switching
```

```
**Disadvantages**
- Blocking sleep reduces performance
- Complex design
```

```
**Summary**
Event loop manages execution of asynchronous tasks.
```

```
---
```

```
## Topic: Asyncio Task Manipulation
```

```
**What I Learned**
I learned how multiple asyncio tasks can run concurrently using Task objects.
```

```
**How to Execute**
python task.py
**Use / Output**
Factorial, Fibonacci, and binomial coefficient are calculated concurrently.
```

```
**When to Use**
When multiple independent computations are required.
```

```
**Advantages**
- Parallel task execution
- Efficient CPU usage
```

```
**Disadvantages**
- Difficult debugging
```

- `Requires async understanding` 

```
**Summary**
Asyncio Tasks allow concurrent execution of multiple coroutines.
```

```
---
```

```
## Topic: Concurrent Futures Pooling
```

```
**What I Learned**
```

```
I learned how ThreadPoolExecutor and ProcessPoolExecutor manage parallel
execution.
```

```
**How to Execute**
python future_pool.py
```

```
**Use / Output**
Program compares sequential, thread pool, and process pool execution times.
```

```
**When to Use**
```

```
When comparing performance of sequential and parallel execution.
```

```
**Advantages**
```

- `Easy parallelism` 

- `Better performance for heavy tasks` 

```
**Disadvantages**
```

```
- Thread overhead
```

- `Process memory usage` 

```
**Summary**
Concurrent futures provide thread and process based parallel execution.
```

```
---
```

