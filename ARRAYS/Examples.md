# Arrays in Java – Clear Examples

## 1. Creating and Printing an Array

```java
public class Main {
    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40, 50};

        System.out.println(arr[0]);
        System.out.println(arr[1]);
        System.out.println(arr[2]);
    }
}
```

### Output

```
10
20
30
```

---

# 2. Taking Input into an Array

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int[] arr = new int[5];

        for(int i = 0; i < 5; i++) {
            arr[i] = sc.nextInt();
        }

        for(int i = 0; i < 5; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}
```

### Input

```
1 2 3 4 5
```

### Output

```
1 2 3 4 5
```

---

# 3. Sum of Array Elements

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {10, 20, 30, 40};

        int sum = 0;

        for(int i = 0; i < arr.length; i++) {
            sum += arr[i];
        }

        System.out.println(sum);
    }
}
```

### Output

```
100
```

---

# 4. Find Largest Element

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {15, 8, 25, 3, 10};

        int max = arr[0];

        for(int i = 1; i < arr.length; i++) {
            if(arr[i] > max) {
                max = arr[i];
            }
        }

        System.out.println(max);
    }
}
```

### Output

```
25
```

---

# 5. Find Smallest Element

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {15, 8, 25, 3, 10};

        int min = arr[0];

        for(int i = 1; i < arr.length; i++) {
            if(arr[i] < min) {
                min = arr[i];
            }
        }

        System.out.println(min);
    }
}
```

### Output

```
3
```

---

# 6. Linear Search

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {10, 20, 30, 40, 50};

        int target = 30;

        for(int i = 0; i < arr.length; i++) {
            if(arr[i] == target) {
                System.out.println("Found at index " + i);
            }
        }
    }
}
```

### Output

```
Found at index 2
```

---

# 7. Reverse an Array

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {1, 2, 3, 4, 5};

        for(int i = arr.length - 1; i >= 0; i--) {
            System.out.print(arr[i] + " ");
        }
    }
}
```

### Output

```
5 4 3 2 1
```

---

# 8. Count Even and Odd Numbers

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {1, 2, 3, 4, 5, 6};

        int even = 0;
        int odd = 0;

        for(int i = 0; i < arr.length; i++) {

            if(arr[i] % 2 == 0)
                even++;
            else
                odd++;
        }

        System.out.println("Even = " + even);
        System.out.println("Odd = " + odd);
    }
}
```

### Output

```
Even = 3
Odd = 3
```

---

# 9. Enhanced For Loop (For-Each Loop)

```java
public class Main {
    public static void main(String[] args) {

        int[] arr = {10, 20, 30, 40};

        for(int num : arr) {
            System.out.println(num);
        }
    }
}
```

### Output

```
10
20
30
40
```

---

# 10. Two-Dimensional Array

```java
public class Main {
    public static void main(String[] args) {

        int[][] arr = {
            {1, 2, 3},
            {4, 5, 6},
            {7, 8, 9}
        };

        for(int i = 0; i < 3; i++) {
            for(int j = 0; j < 3; j++) {
                System.out.print(arr[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```

### Output

```
1 2 3
4 5 6
7 8 9
```

---

# Most Asked Array Programs in Interviews

1. Sum of elements
2. Largest element
3. Smallest element
4. Second largest element
5. Reverse array
6. Linear search
7. Binary search
8. Count even and odd numbers
9. Remove duplicates
10. Sort array (Bubble Sort, Selection Sort)
11. Rotate array
12. Find frequency of elements
13. Merge two arrays
14. Find missing number
15. Kadane's Algorithm (Maximum Subarray Sum)

