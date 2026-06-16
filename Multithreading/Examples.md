# Multithreading in Java – Clear Examples

## 1. Creating a Thread by Extending Thread Class

```java
class MyThread extends Thread {
    public void run() {
        System.out.println("Thread is running...");
    }
}

public class Main {
    public static void main(String[] args) {
        MyThread t1 = new MyThread();
        t1.start();
    }
}
```

### Output

```
Thread is running...
```

---

## 2. Creating a Thread by Implementing Runnable Interface

```java
class MyRunnable implements Runnable {
    public void run() {
        System.out.println("Runnable Thread Running...");
    }
}

public class Main {
    public static void main(String[] args) {
        Thread t1 = new Thread(new MyRunnable());
        t1.start();
    }
}
```

### Output

```
Runnable Thread Running...
```

---

# 3. Multiple Threads Example

```java
class A extends Thread {
    public void run() {
        System.out.println("Thread A");
    }
}

class B extends Thread {
    public void run() {
        System.out.println("Thread B");
    }
}

public class Main {
    public static void main(String[] args) {
        A t1 = new A();
        B t2 = new B();

        t1.start();
        t2.start();
    }
}
```

### Possible Output

```
Thread A
Thread B
```

or

```
Thread B
Thread A
```

(Output order is not guaranteed.)

---

# 4. sleep() Method Example

```java
class MyThread extends Thread {
    public void run() {
        try {
            for(int i=1;i<=3;i++) {
                System.out.println(i);
                Thread.sleep(1000);
            }
        } catch(Exception e) {}
    }
}

public class Main {
    public static void main(String[] args) {
        MyThread t1 = new MyThread();
        t1.start();
    }
}
```

### Output

```
1
(wait 1 sec)
2
(wait 1 sec)
3
```

---

# 5. join() Method Example

```java
class MyThread extends Thread {
    public void run() {
        for(int i=1;i<=3;i++) {
            System.out.println(i);
        }
    }
}

public class Main {
    public static void main(String[] args) throws Exception {
        MyThread t1 = new MyThread();

        t1.start();
        t1.join();

        System.out.println("Main Thread");
    }
}
```

### Output

```
1
2
3
Main Thread
```

`join()` makes the main thread wait until `t1` finishes.

---

# 6. Thread Priority Example

```java
class MyThread extends Thread {
    public void run() {
        System.out.println(getName() + " Priority = " + getPriority());
    }
}

public class Main {
    public static void main(String[] args) {

        MyThread t1 = new MyThread();
        MyThread t2 = new MyThread();

        t1.setPriority(Thread.MIN_PRIORITY);
        t2.setPriority(Thread.MAX_PRIORITY);

        t1.start();
        t2.start();
    }
}
```

### Output

```
Thread-0 Priority = 1
Thread-1 Priority = 10
```

---

# 7. getName() and setName()

```java
class MyThread extends Thread {
    public void run() {
        System.out.println(Thread.currentThread().getName());
    }
}

public class Main {
    public static void main(String[] args) {

        MyThread t1 = new MyThread();
        t1.setName("Java Thread");

        t1.start();
    }
}
```

### Output

```
Java Thread
```

---

# 8. isAlive() Example

```java
class MyThread extends Thread {
    public void run() {
        System.out.println("Running...");
    }
}

public class Main {
    public static void main(String[] args) {

        MyThread t1 = new MyThread();

        System.out.println(t1.isAlive());

        t1.start();

        System.out.println(t1.isAlive());
    }
}
```

### Possible Output

```
false
true
Running...
```

---

# 9. Synchronization Example

```java
class Counter {

    synchronized void printNumbers() {
        for(int i=1;i<=5;i++) {
            System.out.println(i);
        }
    }
}

class A extends Thread {
    Counter c;

    A(Counter c) {
        this.c = c;
    }

    public void run() {
        c.printNumbers();
    }
}

class B extends Thread {
    Counter c;

    B(Counter c) {
        this.c = c;
    }

    public void run() {
        c.printNumbers();
    }
}

public class Main {
    public static void main(String[] args) {

        Counter c = new Counter();

        A t1 = new A(c);
        B t2 = new B(c);

        t1.start();
        t2.start();
    }
}
```

### Output

```
1
2
3
4
5
1
2
3
4
5
```

Synchronization prevents both threads from accessing the method simultaneously.

---

# 10. Daemon Thread Example

```java
class MyThread extends Thread {
    public void run() {
        while(true) {
            System.out.println("Daemon Thread Running");
        }
    }
}

public class Main {
    public static void main(String[] args) {

        MyThread t1 = new MyThread();

        t1.setDaemon(true);

        t1.start();

        System.out.println("Main Thread Ends");
    }
}
```

### Output

```
Main Thread Ends
```

The daemon thread automatically stops when the main thread finishes.

---

## Interview Shortcut

### Thread Creation

```java
class MyThread extends Thread {
    public void run() {
        // task
    }
}
```

### Runnable Creation

```java
class MyRunnable implements Runnable {
    public void run() {
        // task
    }
}
```

### Start Thread

```java
t1.start();
```

### Pause Thread

```java
Thread.sleep(1000);
```

### Wait for Thread

```java
t1.join();
```

### Set Priority

```java
t1.setPriority(10);
```

### Check Alive

```java
t1.isAlive();
```
