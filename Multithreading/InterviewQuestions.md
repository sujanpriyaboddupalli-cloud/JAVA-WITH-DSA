# Multithreading in Java – Interview Questions with Answers

## 1. What is a thread?

A thread is the smallest unit of execution in a process. Multiple threads can run concurrently within the same process.

---

## 2. What is multithreading?

Multithreading is a Java feature that allows multiple threads to execute concurrently, improving performance and responsiveness.

---

## 3. What is the difference between a process and a thread?

| Process             | Thread              |
| ------------------- | ------------------- |
| Independent program | Part of a process   |
| Heavyweight         | Lightweight         |
| Separate memory     | Shared memory       |
| More resource usage | Less resource usage |

---

## 4. How many ways can you create a thread in Java?

Two main ways:

1. Extending Thread class
2. Implementing Runnable interface

---

## 5. Which is better: Thread class or Runnable interface?

Runnable interface is preferred because Java supports single inheritance and a class can extend another class while implementing Runnable.

---

## 6. What is the purpose of the run() method?

The `run()` method contains the code executed by the thread.

---

## 7. What is the purpose of the start() method?

`start()` creates a new thread and internally calls `run()`.

---

## 8. What happens if we call run() directly?

No new thread is created. The method executes like a normal method call.

---

## 9. Difference between start() and run()?

| start()                | run()                      |
| ---------------------- | -------------------------- |
| Creates new thread     | Does not create new thread |
| Executes concurrently  | Executes normally          |
| Calls run() internally | Contains task logic        |

---

## 10. What is the Thread Life Cycle?

1. New
2. Runnable
3. Running
4. Waiting/Blocked
5. Terminated

---

## 11. What is Thread Scheduler?

The JVM component that decides which thread gets CPU time.

---

## 12. What is thread priority?

A value between 1 and 10 that suggests the importance of a thread to the scheduler.

---

## 13. What are the priority constants?

```java
Thread.MIN_PRIORITY = 1
Thread.NORM_PRIORITY = 5
Thread.MAX_PRIORITY = 10
```

---

## 14. What is sleep()?

Used to pause a thread for a specified time.

```java
Thread.sleep(1000);
```

---

## 15. Does sleep() release the lock?

No. The thread sleeps but retains any lock it holds.

---

## 16. What is join()?

Makes one thread wait until another thread finishes execution.

---

## 17. What is yield()?

Temporarily pauses the current thread to give other threads a chance to execute.

---

## 18. What is isAlive()?

Checks whether a thread is still running.

---

## 19. What is synchronization?

A mechanism that allows only one thread at a time to access a shared resource.

---

## 20. Why is synchronization needed?

To prevent:

* Race conditions
* Data inconsistency
* Unexpected results

---

## 21. What is a race condition?

Occurs when multiple threads modify shared data simultaneously, causing unpredictable results.

---

## 22. What is a critical section?

A code segment that accesses shared resources and must not be executed by multiple threads simultaneously.

---

## 23. What is a deadlock?

A situation where two or more threads wait indefinitely for each other’s resources.

### Example

Thread A waits for Thread B's lock and Thread B waits for Thread A's lock.

---

## 24. How can deadlock be prevented?

* Avoid nested locks
* Maintain lock ordering
* Use timeout mechanisms

---

## 25. What is a daemon thread?

A background thread that supports user threads.

### Example

Garbage Collector.

---

## 26. How do you create a daemon thread?

```java
t1.setDaemon(true);
```

Before calling `start()`.

---

## 27. What is the main thread?

The thread automatically created by JVM when a Java program starts.

---

## 28. Can we start a thread twice?

No.

```java
t1.start();
t1.start();
```

Throws:

```java
IllegalThreadStateException
```

---

## 29. What is Thread.currentThread()?

Returns the currently executing thread.

---

## 30. Difference between wait() and sleep()?

| wait()                  | sleep()                 |
| ----------------------- | ----------------------- |
| Belongs to Object class | Belongs to Thread class |
| Releases lock           | Does not release lock   |
| Used in synchronization | Used for delay          |

---

## 31. What is inter-thread communication?

Communication between threads using:

* wait()
* notify()
* notifyAll()

---

## 32. What is notify()?

Wakes up one waiting thread.

---

## 33. What is notifyAll()?

Wakes up all waiting threads.

---

## 34. What is thread safety?

A program is thread-safe if multiple threads can access shared data without producing incorrect results.

---

## 35. What is starvation?

A low-priority thread waits indefinitely because higher-priority threads continuously execute.

---

## 36. What is context switching?

The process of switching CPU execution from one thread to another.

---

## 37. What is concurrency?

Multiple tasks making progress during overlapping time periods.

---

## 38. What is parallelism?

Multiple tasks executing literally at the same time on multiple CPU cores.

---

## 39. Can constructors be synchronized?

No. Constructors cannot be synchronized.

---

## 40. What is the difference between synchronized method and synchronized block?

### Synchronized Method

Locks the entire method.

```java
synchronized void display() {
}
```

### Synchronized Block

Locks only a specific code block.

```java
synchronized(this) {
}
```

More efficient because only part of the code is locked.

---

# Frequently Asked Viva Questions

### Q1: Which method starts a thread?

**Answer:** `start()`

### Q2: Which method contains thread logic?

**Answer:** `run()`

### Q3: Which thread starts first in Java?

**Answer:** Main Thread

### Q4: What is the default priority of a thread?

**Answer:** `5 (NORM_PRIORITY)`

### Q5: Can a class extend Thread and another class simultaneously?

**Answer:** No.

### Q6: Which is preferred for thread creation?

**Answer:** Runnable Interface.

### Q7: What exception occurs when starting a thread twice?

**Answer:** `IllegalThreadStateException`

### Q8: Does Java support multiple inheritance with classes?

**Answer:** No.

### Q9: Name the thread states.

**Answer:** New, Runnable, Running, Waiting/Blocked, Terminated.

### Q10: What is the most common multithreading problem?

**Answer:** Race Condition.
