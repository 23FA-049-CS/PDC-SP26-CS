
## Topic: addTask.py
**What I Learned**

I learned how to create a simple asynchronous task using Celery. The task
performs addition of two numbers and can be executed in the background.

**How to Execute**

Start RabbitMQ server

Run the Celery worker:

celery -A addTask worker --loglevel=info

Run the main program:

python addTaskMain.py

**Use / Output**

The task adds two numbers and returns the result asynchronously.

**When to Use**

When background processing is required without blocking the main application.

**Advantages**

- `Executes tasks asynchronously` 

- `Improves application responsiveness` 

- `Supports distributed task processing` 


**Disadvantages**


- `Requires a message broker such as RabbitMQ` 

- `More complex setup than normal function calls` 


**Summary**

Celery allows Python applications to execute tasks asynchronously using workers
and a message broker.

## Topic: addTaskMain.py

**What I Learned**

I learned how to invoke a Celery task using the `delay()` method and execute it
asynchronously.

**How to Execute**

python addTaskMain.py

**Use / Output**

The program sends an addition task to the Celery worker, which processes it in
the background.

**When to Use**

When tasks need to be executed without waiting for immediate completion.

**Advantages**


- `Easy task submission` 

- `Non-blocking execution` 

- `Suitable for large-scale applications` 


**Disadvantages**


- `Requires active Celery workers` 

- `Results are not immediately available` 


**Summary**

The `delay()` method sends tasks to Celery workers for asynchronous execution.

