```
# Chapter 6 – Socket Programming and Celery in Python
```

```
## Topic: Celery Add Task (addTask.py)
```

```
**What I Learned**
```

```
I learned how to create a simple Celery task that can be executed asynchronously
using a message broker.
```

```
**How to Execute**
```

```
Start RabbitMQ server.
```

```
Run Celery worker:
```

```
celery -A addTask worker --loglevel=info
```

```
**Use / Output**
```

```
The task receives two numbers and returns their sum.
```

```
**When to Use**
```

```
When background task execution is required.
```

```
**Advantages**
```

- `Supports asynchronous execution` 

- `Improves application responsiveness` 

- `Easy task management` 

```
**Disadvantages**
```

- `Requires message broker setup` 

- `Additional configuration needed` 

```
**Summary**
```

```
Celery tasks execute functions asynchronously using workers and brokers.
```

```
## Topic: Running Celery Task (addTaskMain.py)
```

```
**What I Learned**
```

```
I learned how to invoke a Celery task using the delay() method.
```

```
**How to Execute**
```

```
python addTaskMain.py
```

```
**Use / Output**
```

```
The addition task is sent to the Celery worker for execution.
```

```
**When to Use**
```

```
When tasks should run in the background without blocking the main program.
```

```
**Advantages**
```

- `Simple task submission` 

- `Non-blocking execution` 

```
**Disadvantages**
```

- `Requires active Celery worker` 

```
**Summary**
```

```
The delay() method submits tasks for asynchronous execution.
```

```
## Topic: Socket Client (client.py)
```

```
**What I Learned**
```

```
I learned how a TCP client connects to a server and receives data.
```

```
**How to Execute**
```

```
Start server.py first.
```

```
Run:
```

```
python client.py
```

```
**Use / Output**
```

```
The client receives the current time from the server.
```

```
**When to Use**
```

```
When a client needs information from a remote server.
```

```
**Advantages**
```

```
- Simple communication
```

- `Fast data transfer` 

```
**Disadvantages**
```

- `Requires active server` 

- `Connection errors may occur` 

```
**Summary**
```

```
The client establishes a TCP connection and receives data from the server.
```

```
## Topic: File Transfer Client (client2.py)
```

```
**What I Learned**
```

```
I learned how to receive files from a server using socket programming.
```

```
**How to Execute**
Start server2.py first.
```

```
Run:
```

```
python client2.py
```

```
**Use / Output**
```

```
The client downloads a file and saves it as received.txt.
```

```
**When to Use**
```

```
When transferring files over a network.
```

```
**Advantages**
```

- `Supports file sharing` 

- `Simple implementation` 

```
**Disadvantages**
```

- `Limited error handling` 

- `Depends on server availability` 

```
**Summary**
```

```
The client receives file data from the server and stores it locally.
```

```
## Topic: Socket Server (server.py)
```

```
**What I Learned**
```

```
I learned how a TCP server accepts client connections and sends data.
```

```
**How to Execute**
```

```
python server.py
```

```
**Use / Output**
```

```
The server sends the current system time to connected clients.
```

```
**When to Use**
```

```
When providing services to multiple clients.
```

```
**Advantages**
```

```
- Handles client requests
```

```
- Easy to implement
```

```
**Disadvantages**
```

```
- Runs continuously
```

- `Requires open network port` 

```
**Summary**
```

```
The server waits for client connections and sends time information.
```

```
## Topic: File Transfer Server (server2.py)
```

```
**What I Learned**
```

```
I learned how to send files from a server to a client using sockets.
```

```
**How to Execute**
```

```
python server2.py
```

```
**Use / Output**
```

```
The server reads a file and sends its contents to connected clients.
```

```
**When to Use**
```

```
When files need to be shared across systems.
```

```
**Advantages**
```

- `Supports file transmission` 

- `Simple file-sharing mechanism` 

```
**Disadvantages**
```

- `Limited scalability` 

- `No advanced security` 

```
**Summary**
```

```
The server transfers file contents to clients through socket communication.
```

