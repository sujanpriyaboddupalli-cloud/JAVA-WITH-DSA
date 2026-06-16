# Control Statements in Java – Interview Questions with Answers

## 1. What are control statements in Java?

**Answer:**
Control statements control the flow of execution of a program. They decide which statement executes, how many times it executes, and when execution stops.

---

## 2. What are the types of control statements in Java?

**Answer:**

1. Decision Making Statements (`if`, `if-else`, `switch`)    
2. Looping Statements (`for`, `while`, `do-while`)
3. Jump Statements (`break`, `continue`, `return`)

---

## 3. Difference between if and switch?

| if                                 | switch                                      |
| ---------------------------------- | ------------------------------------------- |
| Can evaluate ranges and conditions | Checks fixed values                         |
| Supports logical operators         | Does not support logical operators directly |
| Slower for many conditions         | Faster for multiple options                 |

---

## 4. Difference between while and do-while?

| while                   | do-while                          |
| ----------------------- | --------------------------------- |
| Condition checked first | Condition checked after execution |
| May execute 0 times     | Executes at least once            |

---

## 5. What is an infinite loop?

**Answer:**
A loop that never terminates because its condition always remains true.

```java
while(true)
{
    System.out.println("Hello");
}
```

---

## 6. What is a nested if statement?

**Answer:**
An if statement inside another if statement.

```java
if(age >= 18)
{
    if(citizen)
    {
        System.out.println("Eligible");
    }
}
```

---

## 7. Can switch work with String?

**Answer:**
Yes. Since Java 7, switch supports String values.

```java
String day = "MONDAY";
switch(day)
{
    case "MONDAY":
        System.out.println("Start");
}
```

---

## 8. What is the purpose of break?

**Answer:**
It immediately terminates a loop or switch block.

---

## 9. What is the purpose of continue?

**Answer:**
It skips the current iteration and proceeds with the next iteration.

---

## 10. Can break be used outside a loop?

**Answer:**
No. It causes a compilation error unless used inside a loop or switch.

---

## 11. Can continue be used in a switch statement?

**Answer:**
No. It can only be used inside loops.

---

## 12. Which loop is best when the number of iterations is known?

**Answer:**
`for` loop.

---

## 13. Which loop executes at least once?

**Answer:**
`do-while` loop.

---

## 14. Can we write a for loop without initialization?

**Answer:**
Yes.

```java
int i = 1;

for(; i <= 5; i++)
{
    System.out.println(i);
}
```

---

## 15. Can we write a for loop without condition?

**Answer:**
Yes.

```java
for(;;)
{
    System.out.println("Infinite");
}
```

This creates an infinite loop.

---

## 16. What is the output?

```java
for(int i=0;i<5;i++)
{
    if(i==2)
        break;

    System.out.print(i);
}
```

**Answer:**

```
01
```

---

## 17. What is the output?

```java
for(int i=0;i<5;i++)
{
    if(i==2)
        continue;

    System.out.print(i);
}
```

**Answer:**

```
0134
```

---

## 18. What is fall-through in switch?

**Answer:**
When break is omitted, execution continues to the next case automatically.

```java
switch(1)
{
    case 1:
        System.out.print("A");

    case 2:
        System.out.print("B");
}
```

**Output:**

```
AB
```

---

## 19. What is the output?

```java
int x = 10;

if(x > 5)
    if(x > 8)
        System.out.println("A");
    else
        System.out.println("B");
```

**Answer:**

```
A
```

---

## 20. What is a dangling else problem?

**Answer:**
An else is always associated with the nearest unmatched if.

```java
if(a > b)
    if(a > c)
        System.out.println("A");
    else
        System.out.println("B");
```

The else belongs to the second if.

---

# Complex Interview Questions

## 21. What is the output?

```java
int i = 0;

while(i < 5)
{
    System.out.print(i);
    i++;
}
```

**Answer:**

```
01234
```

---

## 22. What is the output?

```java
int i = 5;

do
{
    System.out.print(i);
}
while(i < 5);
```

**Answer:**

```
5
```

Because do-while executes once before checking the condition.

---

## 23. What is the output?

```java
for(int i=1;i<=3;i++)
{
    for(int j=1;j<=2;j++)
    {
        System.out.print("*");
    }
}
```

**Answer:**

```
******
```

---

## 24. What is the output?

```java
for(int i=1;i<=3;i++)
{
    if(i==2)
        continue;

    System.out.print(i);
}
```

**Answer:**

```
13
```

---

## 25. What is the output?

```java
int x = 5;

switch(x)
{
    case 5:
        System.out.print("A");

    case 6:
        System.out.print("B");

    default:
        System.out.print("C");
}
```

**Answer:**

```
ABC
```

No break statements.

---

## 26. What is the output?

```java
int i;

for(i=1;i<=5;i++);

System.out.println(i);
```

**Answer:**

```
6
```

The semicolon ends the loop.

---

## 27. What is the output?

```java
for(int i=1;i<=3;i++)
{
    System.out.print(i++);
}
```

**Answer:**

```
13
```

Explanation:

* First iteration prints 1, then i becomes 3.
* Second iteration prints 3.

---

## 28. Can switch use double values?

**Answer:**
No.

Valid types:

* byte
* short
* int
* char
* String
* enum

---

## 29. Can return be used in loops?

**Answer:**
Yes.

```java
for(int i=1;i<=5;i++)
{
    if(i==3)
        return;
}
```

Method execution stops completely.

---

## 30. What is the difference between break and return?

| break                          | return                  |
| ------------------------------ | ----------------------- |
| Exits loop/switch only         | Exits entire method     |
| Execution continues after loop | Method ends immediately |

---

## 31. What is labeled break?

```java
outer:
for(int i=1;i<=3;i++)
{
    for(int j=1;j<=3;j++)
    {
        break outer;
    }
}
```

**Answer:**
Exits both loops immediately.

---

## 32. What is labeled continue?

```java
outer:
for(int i=1;i<=3;i++)
{
    for(int j=1;j<=3;j++)
    {
        continue outer;
    }
}
```

**Answer:**
Skips remaining inner loop iterations and continues the outer loop.

---

## 33. Which is faster: switch or if-else ladder?

**Answer:**
For many fixed values, `switch` is generally faster because the JVM can optimize it using jump tables.

---

## 34. What is loop nesting?

**Answer:**
A loop inside another loop.

```java
for(int i=1;i<=3;i++)
{
    for(int j=1;j<=3;j++)
    {
        System.out.print("*");
    }
}
```

---

## 35. What is the time complexity of a nested loop?

```java
for(int i=0;i<n;i++)
{
    for(int j=0;j<n;j++)
    {
    }
}
```

**Answer:**

```
O(n²)
```

---

## 36. What is the output?

```java
int x = 10;

if(x > 5)
{
    System.out.print("A");
}

if(x > 8)
{
    System.out.print("B");
}
```

**Answer:**

```
AB
```

---

## 37. What happens if break is removed from switch?

**Answer:**
Execution falls through to subsequent cases until a break is found or switch ends.

---

## 38. What is the output?

```java
for(int i=1;i<=5;i++)
{
    if(i==4)
        break;

    System.out.print(i);
}
```

**Answer:**

```
123
```

---

## 39. Can a loop exist without a body?

**Answer:**
Yes.

```java
for(int i=0;i<10;i++);
```

This is called an empty loop.

---

## 40. What is the output?

```java
int x = 2;

switch(x)
{
    case 1:
        System.out.print("One");
        break;

    case 2:
        System.out.print("Two");
        break;

    default:
        System.out.print("Default");
}
```

**Answer:**

```
Two
```


