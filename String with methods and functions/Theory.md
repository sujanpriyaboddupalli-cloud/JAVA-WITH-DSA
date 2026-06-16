# String and String Methods in Java (Theory Only)

## 1. What is a String?

A **String** is a sequence of characters used to store text data such as names, messages, addresses, etc.

Example:

* `"Hello"`
* `"Java"`
* `"Sujan"`

In Java, String is an object of the predefined class:

```java
String
```

Strings are **immutable**, meaning once a string object is created, its value cannot be changed.

---

# 2. Features of String

* Used to store textual data.
* Strings are objects in Java.
* Strings are immutable.
* Stored in the String Pool for memory optimization.
* Supports many built-in methods for manipulation.

---

# 3. Ways to Create a String

### Using String Literal

```java
String name = "Java";
```

### Using new Keyword

```java
String name = new String("Java");
```

---

# 4. String Pool

String literals are stored in a special memory area called the **String Constant Pool**.

If two strings have the same value, Java reuses the existing object instead of creating a new one.

Benefits:

* Saves memory.
* Improves performance.

---

# 5. Important String Methods (Theory)

## length()

Returns the number of characters in a string.

**Purpose:** Find string size.

---

## charAt()

Returns the character at a specified index.

**Purpose:** Access a particular character.

---

## substring()

Extracts a portion of a string.

**Purpose:** Retrieve part of a string.

---

## equals()

Compares contents of two strings.

**Purpose:** Check whether two strings have the same value.

---

## equalsIgnoreCase()

Compares two strings without considering uppercase and lowercase letters.

**Purpose:** Case-insensitive comparison.

---

## compareTo()

Compares two strings lexicographically (dictionary order).

**Purpose:** Sorting and ordering strings.

---

## concat()

Joins two strings together.

**Purpose:** String concatenation.

---

## contains()

Checks whether a string contains a specified sequence of characters.

**Purpose:** Searching text.

---

## startsWith()

Checks whether a string starts with a specified prefix.

**Purpose:** Prefix validation.

---

## endsWith()

Checks whether a string ends with a specified suffix.

**Purpose:** Suffix validation.

---

## toUpperCase()

Converts all characters to uppercase.

**Purpose:** Text formatting.

---

## toLowerCase()

Converts all characters to lowercase.

**Purpose:** Standardizing text.

---

## trim()

Removes leading and trailing spaces.

**Purpose:** Cleaning user input.

---

## replace()

Replaces characters or words with new values.

**Purpose:** Text modification.

---

## indexOf()

Returns the first occurrence position of a character or substring.

**Purpose:** Searching location.

---

## lastIndexOf()

Returns the last occurrence position.

**Purpose:** Reverse searching.

---

## isEmpty()

Checks whether a string contains zero characters.

**Purpose:** Empty string validation.

---

## split()

Breaks a string into multiple parts.

**Purpose:** Tokenization and parsing.

---

# 6. String Comparison

### Using == Operator

Compares memory addresses (references).

### Using equals() Method

Compares actual string contents.

**Recommendation:** Use `equals()` for content comparison.

---

# 7. String Concatenation

Combining two or more strings into one string.

Methods:

* `+` Operator
* `concat()` Method

Applications:

* Creating messages
* Generating reports
* Building dynamic text

---

# 8. StringBuffer

A mutable sequence of characters.

Features:

* Can modify content after creation.
* Thread-safe.
* Slower than StringBuilder.

Common Operations:

* append()
* insert()
* delete()
* reverse()

---

# 9. StringBuilder

Also a mutable sequence of characters.

Features:

* Faster than StringBuffer.
* Not thread-safe.
* Preferred for single-threaded applications.

Common Operations:

* append()
* insert()
* delete()
* reverse()

---

# 10. Difference Between String, StringBuffer and StringBuilder

| Feature      | String | StringBuffer | StringBuilder |
| ------------ | ------ | ------------ | ------------- |
| Mutable      | No     | Yes          | Yes           |
| Thread Safe  | No     | Yes          | No            |
| Performance  | Slow   | Medium       | Fast          |
| Memory Usage | More   | Less         | Less          |

---

# 11. Applications of Strings

* User names
* Password validation
* Email processing
* Text editors
* Search engines
* Chat applications
* Web development
* Data processing

---

