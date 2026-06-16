# Control Statements in Java – Examples Only

## 1. if Statement

```java
public class Main {
    public static void main(String[] args) {
        int age = 20;

        if (age >= 18) {
            System.out.println("Eligible to Vote");
        }
    }
}
```

**Output:**

```
Eligible to Vote
```

---

## 2. if-else Statement

```java
public class Main {
    public static void main(String[] args) {
        int num = 7;

        if (num % 2 == 0) {
            System.out.println("Even Number");
        } else {
            System.out.println("Odd Number");
        }
    }
}
```

**Output:**

```
Odd Number
```

---

## 3. else-if Ladder

```java
public class Main {
    public static void main(String[] args) {
        int marks = 85;

        if (marks >= 90) {
            System.out.println("Grade A");
        } else if (marks >= 75) {
            System.out.println("Grade B");
        } else if (marks >= 50) {
            System.out.println("Grade C");
        } else {
            System.out.println("Fail");
        }
    }
}
```

**Output:**

```
Grade B
```

---

## 4. Nested if

```java
public class Main {
    public static void main(String[] args) {
        int age = 20;
        boolean citizen = true;

        if (age >= 18) {
            if (citizen) {
                System.out.println("Can Vote");
            }
        }
    }
}
```

**Output:**

```
Can Vote
```

---

## 5. switch Statement

```java
public class Main {
    public static void main(String[] args) {
        int day = 3;

        switch (day) {
            case 1:
                System.out.println("Monday");
                break;

            case 2:
                System.out.println("Tuesday");
                break;

            case 3:
                System.out.println("Wednesday");
                break;

            default:
                System.out.println("Invalid Day");
        }
    }
}
```

**Output:**

```
Wednesday
```

---

# Looping Statements

## 6. for Loop

```java
public class Main {
    public static void main(String[] args) {

        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }

    }
}
```

**Output:**

```
1
2
3
4
5
```

---

## 7. while Loop

```java
public class Main {
    public static void main(String[] args) {

        int i = 1;

        while (i <= 5) {
            System.out.println(i);
            i++;
        }

    }
}
```

**Output:**

```
1
2
3
4
5
```

---

## 8. do-while Loop

```java
public class Main {
    public static void main(String[] args) {

        int i = 1;

        do {
            System.out.println(i);
            i++;
        } while (i <= 5);

    }
}
```

**Output:**

```
1
2
3
4
5
```

---

# Jump Statements

## 9. break Statement

```java
public class Main {
    public static void main(String[] args) {

        for (int i = 1; i <= 5; i++) {

            if (i == 3) {
                break;
            }

            System.out.println(i);
        }

    }
}
```

**Output:**

```
1
2
```

---

## 10. continue Statement

```java
public class Main {
    public static void main(String[] args) {

        for (int i = 1; i <= 5; i++) {

            if (i == 3) {
                continue;
            }

            System.out.println(i);
        }

    }
}
```

**Output:**

```
1
2
4
5
```

---

## 11. return Statement

```java
public class Main {

    static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {

        int result = add(10, 20);
        System.out.println(result);

    }
}
```

**Output:**

```
30
```

---

## 12. Enhanced for Loop (For-Each)

```java
public class Main {
    public static void main(String[] args) {

        int arr[] = {10, 20, 30, 40};

        for (int num : arr) {
            System.out.println(num);
        }

    }
}
```

**Output:**

```
10
20
30
40
```

