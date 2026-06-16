# Control Statements in Java (Complete Theory)

## What are Control Statements?

Control statements are used to control the flow of execution of a program. They decide:

* Which statement should execute
* How many times a statement should execute
* When execution should stop

Without control statements, Java executes statements sequentially from top to bottom.

---

# Types of Control Statements in Java

Java control statements are divided into 3 categories:

1. Decision Making Statements
2. Looping Statements
3. Jump Statements

---

# 1. Decision Making Statements

These statements help the program make decisions based on conditions.

## a) if Statement

Executes a block of code only if the condition is true.

### Syntax

```java
if(condition)
{
    // code
}
```

### Example

```java
int age = 20;

if(age >= 18)
{
    System.out.println("Eligible to vote");
}
```

### Output

```
Eligible to vote
```

---

## b) if-else Statement

Executes one block if the condition is true and another block if false.

### Syntax

```java
if(condition)
{
    // true block
}
else
{
    // false block
}
```

### Example

```java
int num = 5;

if(num % 2 == 0)
{
    System.out.println("Even");
}
else
{
    System.out.println("Odd");
}
```

### Output

```
Odd
```

---

## c) else-if Ladder

Used when multiple conditions need to be checked.

### Syntax

```java
if(condition1)
{
}
else if(condition2)
{
}
else if(condition3)
{
}
else
{
}
```

### Example

```java
int marks = 85;

if(marks >= 90)
{
    System.out.println("Grade A");
}
else if(marks >= 75)
{
    System.out.println("Grade B");
}
else
{
    System.out.println("Grade C");
}
```

### Output

```
Grade B
```

---

## d) Nested if

An if statement inside another if statement.

### Example

```java
int age = 20;
boolean citizen = true;

if(age >= 18)
{
    if(citizen)
    {
        System.out.println("Can Vote");
    }
}
```

### Output

```
Can Vote
```

---

## e) switch Statement

Used to select one block among many options.

### Syntax

```java
switch(expression)
{
    case value1:
        // code
        break;

    case value2:
        // code
        break;

    default:
        // code
}
```

### Example

```java
int day = 2;

switch(day)
{
    case 1:
        System.out.println("Monday");
        break;

    case 2:
        System.out.println("Tuesday");
        break;

    default:
        System.out.println("Invalid Day");
}
```

### Output

```
Tuesday
```

---

# 2. Looping Statements

Loops execute a block of code repeatedly.

---

## a) for Loop

Used when the number of iterations is known.

### Syntax

```java
for(initialization; condition; increment/decrement)
{
    // code
}
```

### Example

```java
for(int i = 1; i <= 5; i++)
{
    System.out.println(i);
}
```

### Output

```
1
2
3
4
5
```

---

## b) while Loop

Checks the condition first and then executes.

### Syntax

```java
while(condition)
{
    // code
}
```

### Example

```java
int i = 1;

while(i <= 5)
{
    System.out.println(i);
    i++;
}
```

### Output

```
1
2
3
4
5
```

---

## c) do-while Loop

Executes at least once even if the condition is false.

### Syntax

```java
do
{
    // code
}
while(condition);
```

### Example

```java
int i = 1;

do
{
    System.out.println(i);
    i++;
}
while(i <= 5);
```

### Output

```
1
2
3
4
5
```

---

# 3. Jump Statements

Used to transfer control from one part of the program to another.

---

## a) break Statement

Terminates the loop or switch statement immediately.

### Example

```java
for(int i = 1; i <= 5; i++)
{
    if(i == 3)
    {
        break;
    }

    System.out.println(i);
}
```

### Output

```
1
2
```

---

## b) continue Statement

Skips the current iteration and moves to the next iteration.

### Example

```java
for(int i = 1; i <= 5; i++)
{
    if(i == 3)
    {
        continue;
    }

    System.out.println(i);
}
```

### Output

```
1
2
4
5
```

---

## c) return Statement

Terminates a method and returns control to the caller.

### Example

```java
public class Main
{
    static int add()
    {
        return 10 + 20;
    }

    public static void main(String[] args)
    {
        System.out.println(add());
    }
}
```

### Output

```
30
```

---

# Difference Between Loops

| Feature                | for              | while              | do-while        |
| ---------------------- | ---------------- | ------------------ | --------------- |
| Condition Check        | Before execution | Before execution   | After execution |
| Executes At Least Once | No               | No                 | Yes             |
| Best Used When         | Iterations known | Iterations unknown | Must run once   |

---

