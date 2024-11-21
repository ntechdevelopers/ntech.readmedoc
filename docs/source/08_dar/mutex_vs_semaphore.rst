Mutex vs Semaphore
===================================

**What's the difference between a Mutex and a Semaphore?**


Mutexes and Semaphores are synchronization mechanisms used in concurrent programming.
They coordinate access to shared resources and protect them from simultaneous access.

1. Mutex

A mutex, short for mutual exclusion, is like a lock that ensures only one thread can access a resource at any given time. 
Imagine it as a key to a single-person restroom. Only one person can use it at a time, and it stays locked until the person is done. Mutexes are binary—either locked or unlocked.

2. Semaphore

A semaphore is like a parking lot with multiple spots. It uses a counter to track available resources, allowing multiple threads to access them concurrently.
The counter starts at the number of available resources and goes down each time a thread takes a spot. When a thread leaves, the counter goes up. 
Depending on the count, semaphores can allow multiple threads in.

3. Who owns what?

- Mutexes maintain ownership, acquired and released by the same thread or process.
- Semaphores have no inherent concept of ownership. Any thread or process can increment or decrement the semaphore count.

4. When to use each?

- **Mutex**: When you need to ensure only one thread can access a resource at a time.
- **Semaphore**: When you need to allow a limited number of threads to access a resource concurrently.

5. Quick Analogies

- **Mutex**: A single key to a restroom. One person at a time.
- **Semaphore**: A parking lot with limited spaces. Multiple cars can park, but only up to the limit.
