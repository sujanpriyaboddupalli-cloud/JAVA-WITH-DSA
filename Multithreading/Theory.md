# Multithreading in Java (Theory)

## What is Multithreading?

**Multithreading** is a feature in Java that allows a program to execute **multiple threads simultaneously**.

A **thread** is the smallest unit of execution within a process.

### Real-Life Example

Imagine you are:

* Listening to music 🎵
* Downloading a file 📥
* Browsing the internet 🌐

All these tasks run at the same time. This is similar to multithreading.

---

# Why Multithreading?

### Advantages

1. Better CPU utilization
2. Faster execution of programs
3. Improved performance
4. Allows concurrent execution of tasks
5. Enhances user experience in applications

---

# Process vs Thread

| Process                                      | Thread                      |
| -------------------------------------------- | --------------------------- |
| Independent program                          | Part of a process           |
| Heavyweight                                  | Lightweight                 |
| More memory required                         | Less memory required        |
| Communication is slower                      | Communication is faster     |
| Example: Chrome and VS Code running together | Multiple tabs inside Chrome |

---

# Thread Life Cycle

A thread passes through the following states:

## 1. New State

Thread object is created but not started.

## 2. Runnable State

Thread is ready to run and waiting for CPU.

## 3. Running State

CPU executes the thread.

## 4. Blocked/Waiting State

Thread waits for a resource or another thread.

## 5. Terminated (Dead) State

Thread completes execution.

### Flow

```
New
 ↓
Runnable
 ↓
Running
 ↓
Waiting/Blocked
 ↓
Terminated
```

---

# Ways to Create a Thread

## 1. By Extending Thread Class

A class extends the Thread class and overrides the run() method.

### Features

* Simple approach
* Cannot extend another class because Java doesn't support multiple inheritance

---

## 2. By Implementing Runnable Interface

A class implements Runnable and defines the run() method.

### Features

* Better approach
* Supports inheritance of other classes
* Most commonly used

---

# Main Thread

Every Java program starts with a **Main Thread**.

```java
public static void main(String[] args)
```

The JVM automatically creates this thread.

### Responsibilities

* Starts program execution
* Creates other threads
* Terminates after completing tasks

---

# Thread Methods

## start()

Starts a new thread.

### Purpose

Creates a separate execution path.

---

## run()

Contains the code executed by the thread.

### Purpose

Defines thread task.

---

## sleep()

Pauses a thread for a specified time.

### Purpose

Temporarily stops execution.

---

## join()

Makes one thread wait until another thread finishes.

### Purpose

Synchronization between threads.

---

## yield()

Temporarily gives CPU to another thread.

### Purpose

Improves thread scheduling.

---

## isAlive()

Checks whether a thread is still running.

### Returns

* true → running
* false → terminated

---

## getName()

Returns thread name.

---

## setName()

Changes thread name.

---

## getPriority()

Returns thread priority.

---

## setPriority()

Sets thread priority.

---

# Thread Priority

Java provides priorities from:

```
1 to 10
```

### Constants

| Constant      | Value |
| ------------- | ----- |
| MIN_PRIORITY  | 1     |
| NORM_PRIORITY | 5     |
| MAX_PRIORITY  | 10    |

### Purpose

Helps JVM decide which thread gets CPU first.

---

# Synchronization

## Definition

Synchronization is a mechanism used to control access to shared resources by multiple threads.

### Why Needed?

Without synchronization:

* Data inconsistency occurs
* Race conditions occur
* Unexpected output is produced

### Benefits

* Data integrity
* Thread safety
* Prevents conflicts

---

# Race Condition

A race condition occurs when multiple threads access and modify shared data simultaneously, causing unpredictable results.

### Example

Two threads updating the same bank account balance at the same time.

---

# Deadlock

## Definition

Deadlock occurs when two or more threads wait indefinitely for resources held by each other.

### Characteristics

* Threads stop progressing
* Program hangs
* Resources remain locked

---

# Inter-Thread Communication

Java provides communication between threads using:

* wait()
* notify()
* notifyAll()

### Purpose

Allows threads to coordinate with each other efficiently.

---

# Daemon Thread

A daemon thread runs in the background and supports user threads.

### Examples

* Garbage Collector
* Background services

### Characteristics

* Low priority
* Automatically terminates when all user threads finish

---

# Thread Safety

A program is thread-safe if multiple threads can access shared resources without causing incorrect results.

### Achieved Using

* Synchronization
* Locks
* Concurrent collections

---

# Multitasking Types

## 1. Process-Based Multitasking

Multiple processes run simultaneously.

### Example

* Chrome
* VS Code
* Spotify

running together.

---

## 2. Thread-Based Multitasking

Multiple threads run within the same process.

### Example

Inside a browser:

* One thread loads images
* One thread loads videos
* One thread handles user input

---

# Benefits of Multithreading

1. Better responsiveness
2. Efficient CPU utilization
3. Resource sharing
4. Faster execution
5. Concurrent task processing
6. Reduced idle time

---

# Limitations of Multithreading

1. Complex debugging
2. Synchronization overhead
3. Deadlock possibility
4. Race conditions
5. Increased program complexity

---

# Interview Definition

**Multithreading:**
Multithreading is a Java feature that allows multiple threads to execute concurrently within a single process, improving performance, responsiveness, and CPU utilization.
