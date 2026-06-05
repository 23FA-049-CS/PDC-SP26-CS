```
## Topic: client.py
```

```
**What I Learned**
```

```
I learned how a Pyro4 client connects to a remote server object and invokes
methods remotely.
```

```
**How to Execute**
```

```
Start the Pyro Name Server:
```

```
pyro4-ns
```

```
Start the server:
```

```
python server.py
```

```
Run the client:
```

```
python client.py
```

```
**Use / Output**
```

```
The client sends a user's name to the server and receives a welcome message.
```

```
**When to Use**
```

```
When a client application needs to communicate with a remote server.
```

```
**Advantages**
```

- `Simple remote method invocation` 

- `Easy client-server communication` 

- `Hides network communication details` 

```
**Disadvantages**
```

- `Requires a running Name Server` 

- `Dependent on network connectivity` 

```
**Summary**
Pyro4 Client connects to remote objects and executes methods remotely.
```

```
## Topic: server.py
```

```
**What I Learned**
I learned how to create and expose remote objects using a Pyro4 server.
```

```
**How to Execute**
Start the Pyro Name Server:
```

```
pyro4-ns
```

```
Run:
```

```
python server.py
```

```
**Use / Output**
The server waits for client requests and returns welcome messages.
```

```
**When to Use**
When providing remote services to clients.
```

```
**Advantages**
- Easy object sharing
- Supports distributed systems
```

- `Simple implementation` 

```
**Disadvantages**
```

- `Requires server management` 

- `Network overhead` 

```
**Summary**
```

```
Pyro4 Server exposes Python objects for remote access.
```

## `## Topic: chainTopology.py` 

```
**What I Learned**
```

```
I learned how multiple remote servers can be connected together in a chain
topology.
```

```
**How to Execute**
```

```
python chainTopology.py
```

```
(Used with Server1, Server2, and Server3)
```

```
**Use / Output**
```

```
Messages are forwarded through multiple servers and returned to the client.
```

```
**When to Use**
```

```
When requests need to pass through multiple distributed nodes.
```

```
**Advantages**
```

- `Distributed processing` 

- `Modular architecture` 

- `Easy scalability` 

```
**Disadvantages**
```

- `Complex setup` 

- `Dependency on multiple servers` 

```
**Summary**
Chain topology forwards requests through multiple connected servers.
```

```
## Topic: clientChain.py
```

```
**What I Learned**
```

```
I learned how a client can start communication through the first node in a chain
topology.
```

```
**How to Execute**
```

```
python clientChain.py
```

```
**Use / Output**
```

```
The client sends a message and receives the complete chain traversal result.
```

```
**When to Use**
When testing chain-based distributed communication.
```

```
**Advantages**
```

- `Simple request initiation` 

- `Demonstrates distributed communication` 

```
**Disadvantages**
```

- `Requires all chain servers to be running` 

```
**Summary**
The client starts message processing through the chain topology.
```

```
## Topic: Chain Server 1 (server1.py)
```

```
**What I Learned**
```

```
I learned how to create the first node of a distributed chain topology.
```

```
**How to Execute**
python server1.py
```

```
**Use / Output**
Receives requests and forwards them to Server 2.
```

```
**When to Use**
As the starting node in a chain network.
```

```
**Advantages**
- Organized request forwarding
```

```
- Supports distributed execution
```

```
**Disadvantages**
```

```
- Depends on next server availability
```

```
**Summary**
Server 1 acts as the first node in the chain.
```

```
## Topic: server2.py
```

```
**What I Learned**
I learned how an intermediate server forwards requests to the next node.
```

```
**How to Execute**
python server2.py
```

```
**Use / Output**
Receives requests from Server 1 and forwards them to Server 3.
```

```
**When to Use**
As a middle node in a distributed chain.
```

```
**Advantages**
- Supports message routing
```

```
- Improves modularity
```

```
**Disadvantages**
```

```
- Failure affects chain execution
```

```
**Summary**
Server 2 acts as an intermediate forwarding node.
```

```
## Topic: Chain Server 3 (server3.py)
```

```
**What I Learned**
I learned how the final server closes the chain and returns results.
```

```
**How to Execute**
python server3.py
```

```
**Use / Output**
Receives requests from Server 2 and returns the final result back through the
chain.
```

```
**When to Use**
As the final node in a chain topology.
```

```
**Advantages**
- Completes processing cycle
```

- `Returns final response` 

```
**Disadvantages**
```

- `Entire chain depends on its availability` 

```
**Summary**
Server 3 completes the chain topology and returns results.
```

