# CS402 - Operating Systems

Concurrency, deadlock control, synchronization, process and thread scheduling, memory management, file systems, security and access control, communication and networking, distributed file systems, data management.

> The specs and implementation of projects in this course are private. While I can publicily describe the projects in the later sections, the implementations are private. Although, they can be shared privately for anyone who wishes to see the implementation and understand the scope of my work. 

## Token Bucket Filter Emulator
This project emulates a commonly used Network Shaper known as the Token Bucket Filter. 
- This emulation is Time-Driven and uses multiple threads to drive 1 Packet Generator, 1 Token Generator and 2 Servers.
- Shared resources (Queues, System calls) are protected by a Mutex.
- The servers perform a blocking wait to service a packet using conditional variables.
- A signal handling thread also watches for SIGINT to cleanly halt the simulation on user request.
  - Predictable thread cancellation is used by allowing the threads to stop at specific cancellation points. 
- The emulation statistics are presented to the user at the end of the simulation.

> Further details of the project are available on [request](https://github.com/swanav/cs402-project-fall-23/issues/new/choose).

## The Weenix Kernel

### Process Management - (Processes, Kernel Threads, Scheduler, Mutex)


