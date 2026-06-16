# Arrays in Java – Interview Questions with Answers

## 1. What is an array in Java?

**Answer:**
An array is a collection of elements of the same data type stored under a single variable name.

```java
int[] arr = {10, 20, 30};
```

---

## 2. Why are arrays used?

**Answer:**

* Store multiple values in one variable.
* Easy access using indexes.
* Reduces code complexity.

---

## 3. What is the index of the first element in an array?

**Answer:**
Index starts from **0**.

```java
int[] arr = {10,20,30};
System.out.println(arr[0]);
```

Output:

```
10
```

---

## 4. How do you find the size of an array?

**Answer:**

```java
arr.length
```

Example:

```java
int[] arr = {1,2,3,4};
System.out.println(arr.length);
```

Output:

```
4
```

---

## 5. Can an array store different data types?

**Answer:**
No. An array can store only one type of data.

```java
int[] arr = {1,2,3};
```

Valid

```java
int[] arr = {1,"Hello"};
```

Invalid

---

## 6. What are the default values of array elements?

**Answer:**

| Data Type | Default Value |
| --------- | ------------- |
| int       | 0             |
| double    | 0.0           |
| boolean   | false         |
| char      | '\u0000'      |
| String    | null          |

---

## 7. Difference between Array and ArrayList?

| Array                  | ArrayList                     |
| ---------------------- | ----------------------------- |
| Fixed size             | Dynamic size                  |
| Faster                 | Slightly slower               |
| Stores primitive types | Stores objects                |
| Part of Java language  | Part of Collections Framework |

---

## 8. What is ArrayIndexOutOfBoundsException?

**Answer:**
Occurs when accessing an invalid index.

```java
int[] arr = {10,20,30};
System.out.println(arr[5]);
```

---

## 9. How do you traverse an array?

**Answer:**

```java
for(int i=0;i<arr.length;i++){
    System.out.println(arr[i]);
}
```

---

## 10. What is a multidimensional array?

**Answer:**
An array containing another array.

```java
int[][] arr = new int[3][3];
```

---

# Intermediate Interview Questions

## 11. How do you find the largest element in an array?

```java
int max = arr[0];

for(int i=1;i<arr.length;i++){
    if(arr[i] > max){
        max = arr[i];
    }
}
```

---

## 12. How do you find the smallest element?

```java
int min = arr[0];

for(int i=1;i<arr.length;i++){
    if(arr[i] < min){
        min = arr[i];
    }
}
```

---

## 13. How do you calculate the sum of array elements?

```java
int sum = 0;

for(int num : arr){
    sum += num;
}
```

---

## 14. How do you reverse an array?

```java
for(int i=arr.length-1;i>=0;i--){
    System.out.print(arr[i]+" ");
}
```

---

## 15. What is Linear Search?

**Answer:**
Checking elements one by one until the target is found.

Time Complexity:

```
O(n)
```

---

## 16. What is Binary Search?

**Answer:**
Searches a sorted array by repeatedly dividing it into halves.

Time Complexity:

```
O(log n)
```

---

## 17. Which search is faster?

**Answer:**
Binary Search is faster.

| Search        | Complexity |
| ------------- | ---------- |
| Linear Search | O(n)       |
| Binary Search | O(log n)   |

---

## 18. How do you count even numbers in an array?

```java
int count = 0;

for(int num : arr){
    if(num % 2 == 0)
        count++;
}
```

---

## 19. How do you count odd numbers?

```java
int count = 0;

for(int num : arr){
    if(num % 2 != 0)
        count++;
}
```

---

## 20. What is the difference between `length` and `length()`?

**Answer:**

| length          | length()         |
| --------------- | ---------------- |
| Used for arrays | Used for Strings |
| Property        | Method           |

Example:

```java
arr.length
```

```java
str.length()
```

---

# Advanced Interview Questions

## 21. Find Second Largest Element

```java
int largest = Integer.MIN_VALUE;
int second = Integer.MIN_VALUE;

for(int num : arr){
    if(num > largest){
        second = largest;
        largest = num;
    }
    else if(num > second && num != largest){
        second = num;
    }
}
```

---

## 22. Remove Duplicates from a Sorted Array

**Approach:**

* Use two pointers.
* Keep unique elements only.

Time Complexity:

```
O(n)
```

---

## 23. Rotate Array by One Position

Input:

```
1 2 3 4 5
```

Output:

```
5 1 2 3 4
```

---

## 24. Find Missing Number

Input:

```
1 2 3 5
```

Output:

```
4
```

Formula:

```java
n*(n+1)/2
```

---

## 25. What happens when array size is exceeded?

**Answer:**
Java throws:

```java
ArrayIndexOutOfBoundsException
```

---

## 26. Are arrays objects in Java?

**Answer:**
Yes.

```java
int[] arr = new int[5];
```

Arrays are created using `new`, meaning they are objects.

---

## 27. Can array size be changed after creation?

**Answer:**
No.

```java
int[] arr = new int[5];
```

Size remains fixed.

---

## 28. What is Jagged Array?

**Answer:**
A 2D array where rows have different lengths.

```java
int[][] arr = {
    {1,2},
    {3,4,5},
    {6}
};
```

---

## 29. What is the time complexity of accessing an element?

```java
arr[i]
```

**Answer:**

```
O(1)
```

Because arrays provide direct access.

---

## 30. Why are arrays fast?

**Answer:**

* Contiguous memory allocation.
* Direct index access.
* Constant-time retrieval.

---

