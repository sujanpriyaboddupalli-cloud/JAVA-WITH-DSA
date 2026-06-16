

# Java Basics - Theory

## 1. What is Java?

Java is a high-level, object-oriented, platform-independent programming language developed by James Gosling in 1995.

### Features of Java

* Simple
* Object-Oriented
* Platform Independent
* Secure
* Robust
* Portable
* Multithreaded
* Distributed
* Dynamic

---

## 2. History of Java

* Developed by Sun Microsystems in 1995.
* Initially called **Oak**.
* Later renamed **Java**.
* Now maintained by [Oracle Corporation](https://www.oracle.com?utm_source=chatgpt.com).

---

## 3. Java Architecture

### JDK (Java Development Kit)

A complete package used to develop Java applications.

Contains:

* JRE
* Compiler (javac)
* Debugger
* Documentation tools

### JRE (Java Runtime Environment)

Provides environment to run Java programs.

Contains:

* JVM
* Libraries

### JVM (Java Virtual Machine)

Executes Java bytecode.

**Flow:**

```
Java Program
     ↓
Compiler (javac)
     ↓
Bytecode (.class)
     ↓
JVM
     ↓
Output
```

---

## 4. Java Program Structure

Every Java program contains:

### Package Declaration

Defines package name.

### Import Statements

Imports built-in libraries.

### Class Declaration

Contains program code.

### Main Method

Starting point of execution.

---

## 5. Java Tokens

Smallest individual units of a program.

### Types of Tokens

#### Keywords

Reserved words with predefined meaning.

Examples:

```
class
public
static
void
if
else
for
while
return
```

#### Identifiers

Names given to variables, methods, classes.

Example:

```
studentName
age
Employee
```

#### Literals

Fixed values.

Example:

```
100
3.14
'A'
"Hello"
true
```

#### Operators

Perform operations.

Example:

```
+
-
*
/
%
```

#### Separators

Symbols used to separate statements.

Example:

```
;
{}
()
[]
,
.
```

---

## 6. Data Types in Java

### Primitive Data Types

| Data Type | Size    | Example |
| --------- | ------- | ------- |
| byte      | 1 Byte  | 10      |
| short     | 2 Bytes | 100     |
| int       | 4 Bytes | 1000    |
| long      | 8 Bytes | 100000  |
| float     | 4 Bytes | 12.5f   |
| double    | 8 Bytes | 12.567  |
| char      | 2 Bytes | 'A'     |
| boolean   | 1 Bit   | true    |

### Non-Primitive Data Types

* String
* Array
* Class
* Interface
* Object

---

## 7. Variables

Variables are containers used to store data.

### Types

#### Local Variable

Declared inside a method.

#### Instance Variable

Declared inside class but outside method.

#### Static Variable

Declared using static keyword.

---

## 8. Type Casting

### Widening Casting

Small → Large

```
int → long → float → double
```

### Narrowing Casting

Large → Small

```
double → float → int
```

---

## 9. Operators in Java

### Arithmetic Operators

```
+
-
*
/
%
```

### Relational Operators

```
==
!=
>
<
>=
<=
```

### Logical Operators

```
&&
||
!
```

### Assignment Operators

```
=
+=
-=
*=
/=
```

### Increment and Decrement

```
++
--
```

### Bitwise Operators

```
&
|
^
~
<<
>>
```

### Ternary Operator

```
condition ? true : false
```

---

## 10. Control Statements

### Selection Statements

#### if

#### if-else

#### else-if

#### switch

Used for decision making.

---

### Looping Statements

#### for Loop

Used when number of iterations is known.

#### while Loop

Checks condition first.

#### do-while Loop

Executes at least once.

---

### Jump Statements

#### break

Terminates loop.

#### continue

Skips current iteration.

#### return

Returns value from method.

---

## 11. Arrays

Array stores multiple values of same data type in a single variable.

### Advantages

* Easy data storage
* Fast access
* Less memory usage

### Types

* Single Dimensional Array
* Multidimensional Array

---

## 12. Strings

String is a sequence of characters.

### Features

* Immutable
* Stored as objects
* Belongs to String class

### Common String Methods

| Method        | Purpose               |
| ------------- | --------------------- |
| length()      | Length of string      |
| charAt()      | Character at position |
| substring()   | Extract part          |
| equals()      | Compare strings       |
| toUpperCase() | Convert to upper      |
| toLowerCase() | Convert to lower      |
| trim()        | Remove spaces         |
| replace()     | Replace characters    |
| contains()    | Check existence       |

---

## 13. Methods (Functions)

Method is a block of code that performs a specific task.

### Advantages

* Reusability
* Easy maintenance
* Modular programming

### Types

* User-defined methods
* Built-in methods

---

## 14. Object-Oriented Programming (OOP)

### Class

Blueprint of an object.

### Object

Instance of a class.

### Encapsulation

Wrapping data and methods together.

### Inheritance

One class acquires properties of another class.

### Polymorphism

One method behaves differently.

### Abstraction

Showing essential details only.

---

## 15. Exception Handling

Used to handle runtime errors.

### Keywords

```
try
catch
finally
throw
throws
```

### Benefits

* Prevents program crash
* Maintains normal flow

---

## 16. Multithreading

Executing multiple threads simultaneously.

### Advantages

* Better performance
* Resource sharing
* Concurrent execution

### Thread Lifecycle

```
New
 ↓
Runnable
 ↓
Running
 ↓
Waiting
 ↓
Terminated
```

---

## 17. Collections Framework

Used to store and manage groups of objects.

### Important Interfaces

* List
* Set
* Queue
* Map

### Common Classes

* ArrayList
* LinkedList
* HashSet
* HashMap
* PriorityQueue

---

## 18. Java Memory Management

### Stack Memory

Stores local variables and method calls.

### Heap Memory

Stores objects and instance variables.

### Garbage Collection

Automatically removes unused objects.

---

## 19. Java Packages

Package is a collection of related classes and interfaces.

### Types

* Built-in Packages
* User-defined Packages

Examples:

```
java.lang
java.util
java.io
java.sql
```

---

## 20. Why Java is Platform Independent?

Java source code is compiled into **Bytecode**.

The bytecode runs on JVM.

Since JVM is available for different operating systems, the same Java program can run anywhere.

**"Write Once, Run Anywhere (WORA)"**. 🚀

