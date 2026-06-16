# String Methods and Functions in Java (Examples Only)

## 1. Creating a String

```java
String name = "Java";
System.out.println(name);
```

---

## 2. length()

```java
String str = "Hello";
System.out.println(str.length());
```

**Output**

```
5
```

---

## 3. charAt()

```java
String str = "Java";
System.out.println(str.charAt(2));
```

**Output**

```
v
```

---

## 4. substring()

```java
String str = "Programming";
System.out.println(str.substring(3));
System.out.println(str.substring(3, 7));
```

**Output**

```
gramming
gram
```

---

## 5. equals()

```java
String s1 = "Java";
String s2 = "Java";

System.out.println(s1.equals(s2));
```

**Output**

```
true
```

---

## 6. equalsIgnoreCase()

```java
String s1 = "JAVA";
String s2 = "java";

System.out.println(s1.equalsIgnoreCase(s2));
```

**Output**

```
true
```

---

## 7. compareTo()

```java
String s1 = "Apple";
String s2 = "Banana";

System.out.println(s1.compareTo(s2));
```

**Output**

```
-1
```

---

## 8. concat()

```java
String first = "Hello ";
String second = "Java";

System.out.println(first.concat(second));
```

**Output**

```
Hello Java
```

---

## 9. contains()

```java
String str = "Welcome to Java";

System.out.println(str.contains("Java"));
```

**Output**

```
true
```

---

## 10. startsWith()

```java
String str = "Programming";

System.out.println(str.startsWith("Pro"));
```

**Output**

```
true
```

---

## 11. endsWith()

```java
String str = "Programming";

System.out.println(str.endsWith("ing"));
```

**Output**

```
true
```

---

## 12. toUpperCase()

```java
String str = "java";

System.out.println(str.toUpperCase());
```

**Output**

```
JAVA
```

---

## 13. toLowerCase()

```java
String str = "JAVA";

System.out.println(str.toLowerCase());
```

**Output**

```
java
```

---

## 14. trim()

```java
String str = "   Java   ";

System.out.println(str.trim());
```

**Output**

```
Java
```

---

## 15. replace()

```java
String str = "I Love Java";

System.out.println(str.replace("Java", "Python"));
```

**Output**

```
I Love Python
```

---

## 16. indexOf()

```java
String str = "Programming";

System.out.println(str.indexOf('g'));
```

**Output**

```
3
```

---

## 17. lastIndexOf()

```java
String str = "Programming";

System.out.println(str.lastIndexOf('g'));
```

**Output**

```
10
```

---

## 18. isEmpty()

```java
String str = "";

System.out.println(str.isEmpty());
```

**Output**

```
true
```

---

## 19. split()

```java
String str = "Java,Python,C++";

String[] arr = str.split(",");

for(String s : arr)
{
    System.out.println(s);
}
```

**Output**

```
Java
Python
C++
```

---

## 20. == vs equals()

```java
String s1 = new String("Java");
String s2 = new String("Java");

System.out.println(s1 == s2);
System.out.println(s1.equals(s2));
```

**Output**

```
false
true
```

---

# StringBuilder Examples

## append()

```java
StringBuilder sb = new StringBuilder("Java");

sb.append(" Programming");

System.out.println(sb);
```

**Output**

```
Java Programming
```

---

## insert()

```java
StringBuilder sb = new StringBuilder("Jva");

sb.insert(1, "a");

System.out.println(sb);
```

**Output**

```
Java
```

---

## delete()

```java
StringBuilder sb = new StringBuilder("Java Programming");

sb.delete(4, 16);

System.out.println(sb);
```

**Output**

```
Java
```

---

## reverse()

```java
StringBuilder sb = new StringBuilder("Java");

System.out.println(sb.reverse());
```

**Output**

```
avaJ
```

---

# StringBuffer Examples

## append()

```java
StringBuffer sb = new StringBuffer("Hello");

sb.append(" World");

System.out.println(sb);
```

**Output**

```
Hello World
```

---

## reverse()

```java
StringBuffer sb = new StringBuffer("Java");

System.out.println(sb.reverse());
```

**Output**

```
avaJ
```

These examples cover the most commonly asked String, StringBuilder, and StringBuffer methods in Java interviews and lab exams.
