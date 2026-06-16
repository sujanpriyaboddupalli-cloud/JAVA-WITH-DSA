# Arrays in Java (Theory)

## What is an Array?

An **array** is a collection of elements of the **same data type** stored in **contiguous memory locations**.

Instead of creating many variables separately, an array allows us to store multiple values under a single name.

### Example

Without array:

```java
int mark1 = 90;
int mark2 = 85;
int mark3 = 95;
```

With array:

```java
int[] marks = {90, 85, 95};
```

---

# Why Do We Need Arrays?

* Store multiple values using one variable.
* Reduce code complexity.
* Easy access using index numbers.
* Useful for searching, sorting, and data processing.

---

# Features of Arrays

1. Fixed size.
2. Stores similar data types only.
3. Index starts from 0.
4. Stored in contiguous memory.
5. Faster access using index.

---

# Array Declaration

### Syntax

```java
datatype[] arrayName;
```

or

```java
datatype arrayName[];
```

### Example

```java
int[] numbers;
String[] names;
```

---

# Array Creation

### Syntax

```java
arrayName = new datatype[size];
```

### Example

```java
int[] numbers = new int[5];
```

This creates an array capable of storing 5 integers.

---

# Array Initialization

### Method 1

```java
int[] arr = {10, 20, 30, 40, 50};
```

### Method 2

```java
int[] arr = new int[5];
arr[0] = 10;
arr[1] = 20;
arr[2] = 30;
arr[3] = 40;
arr[4] = 50;
```

---

# Indexing in Array

Each element is identified by an index.

```java
int[] arr = {10,20,30,40,50};
```

| Index | Value |
| ----- | ----- |
| 0     | 10    |
| 1     | 20    |
| 2     | 30    |
| 3     | 40    |
| 4     | 50    |

Accessing element:

```java
System.out.println(arr[2]);
```

Output:

```
30
```

---

# Types of Arrays in Java

## 1. One-Dimensional Array (1D)

Stores elements in a single row.

```java
int[] arr = {1,2,3,4,5};
```

---

## 2. Two-Dimensional Array (2D)

Stores data in rows and columns.

```java
int[][] matrix = new int[3][3];
```

Example:

|   |   |   |
| - | - | - |
| 1 | 2 | 3 |
| 4 | 5 | 6 |
| 7 | 8 | 9 |

---

## 3. Multidimensional Array

More than two dimensions.

```java
int[][][] data = new int[2][3][4];
```

Used in advanced applications like graphics and scientific computations.

---

# Default Values in Arrays

When an array is created using `new`, Java assigns default values.

| Data Type     | Default Value |
| ------------- | ------------- |
| int           | 0             |
| long          | 0             |
| float         | 0.0           |
| double        | 0.0           |
| char          | '\u0000'      |
| boolean       | false         |
| String/Object | null          |

Example:

```java
int[] arr = new int[3];
```

Output:

```
0 0 0
```

---

# Length Property

Used to find the size of an array.

### Syntax

```java
arrayName.length
```

### Example

```java
int[] arr = {10,20,30,40};

System.out.println(arr.length);
```

Output:

```
4
```

---

# Advantages of Arrays

1. Easy storage of multiple values.
2. Fast access using index.
3. Less code.
4. Efficient memory management.
5. Useful in sorting and searching algorithms.

---

# Disadvantages of Arrays

1. Fixed size.
2. Cannot store different data types together.
3. Insertion and deletion are difficult.
4. Memory may be wasted if array size is larger than needed.

---

# ArrayIndexOutOfBoundsException

Occurs when accessing an invalid index.

Example:

```java
int[] arr = {10,20,30};

System.out.println(arr[5]);
```

Output:

```
ArrayIndexOutOfBoundsException
```

Because valid indexes are only:

```
0, 1, 2
```

---

# Important Points for Interviews

1. Arrays store elements of the same data type.
2. Array index starts from 0.
3. Array size is fixed after creation.
4. Arrays are objects in Java.
5. `length` gives the size of an array.
6. Arrays can be single-dimensional, two-dimensional, or multidimensional.
7. Invalid index access causes `ArrayIndexOutOfBoundsException`.
8. Java arrays are dynamically allocated memory.
9. Default values are assigned automatically.
10. Arrays are stored in contiguous memory locations.

This theory is suitable for your GitHub **DSA with Java → Arrays → Theory.md** file.
