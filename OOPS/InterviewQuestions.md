# OOPS in Java - Interview Questions with Answers

## 1. What is OOPS?

**Answer:**
OOPS (Object-Oriented Programming System) is a programming paradigm that uses objects and classes to organize code. The four pillars are Encapsulation, Inheritance, Polymorphism, and Abstraction.

---

## 2. What are the four pillars of OOPS?

**Answer:**

1. Encapsulation
2. Inheritance
3. Polymorphism
4. Abstraction

---

## 3. What is a Class?

**Answer:**
A class is a blueprint or template used to create objects.

---

## 4. What is an Object?

**Answer:**
An object is an instance of a class that contains state (data) and behavior (methods).

---

## 5. What is the difference between Class and Object?

**Answer:**

| Class               | Object           |
| ------------------- | ---------------- |
| Blueprint           | Instance         |
| Logical entity      | Physical entity  |
| No memory allocated | Memory allocated |

---

## 6. What is Encapsulation?

**Answer:**
Encapsulation is wrapping data and methods into a single unit and restricting direct access to data using access modifiers.

---

## 7. How is Encapsulation achieved in Java?

**Answer:**
By declaring variables as `private` and accessing them using getter and setter methods.

---

## 8. What is Inheritance?

**Answer:**
Inheritance allows one class to acquire properties and methods of another class using the `extends` keyword.

---

## 9. Why is Inheritance used?

**Answer:**

* Code Reusability
* Reduces Redundancy
* Easier Maintenance

---

## 10. What are the types of Inheritance in Java?

**Answer:**

* Single
* Multilevel
* Hierarchical
* Multiple (through Interfaces)
* Hybrid (through Interfaces)

---

## 11. Does Java support Multiple Inheritance?

**Answer:**
No, Java does not support multiple inheritance through classes because of the Diamond Problem. It supports it through interfaces.

---

## 12. What is Polymorphism?

**Answer:**
Polymorphism means one interface with multiple forms.

---

## 13. What are the types of Polymorphism?

**Answer:**

1. Compile-Time Polymorphism (Method Overloading)
2. Runtime Polymorphism (Method Overriding)

---

## 14. What is Method Overloading?

**Answer:**
Having multiple methods with the same name but different parameters in the same class.

---

## 15. What is Method Overriding?

**Answer:**
Providing a new implementation of a parent class method in the child class.

---

## 16. Difference between Overloading and Overriding?

| Overloading          | Overriding           |
| -------------------- | -------------------- |
| Same class           | Parent-Child classes |
| Compile Time         | Runtime              |
| Different Parameters | Same Parameters      |

---

## 17. What is Abstraction?

**Answer:**
Abstraction hides implementation details and shows only essential features.

---

## 18. How is Abstraction achieved in Java?

**Answer:**

* Abstract Classes
* Interfaces

---

## 19. What is an Abstract Class?

**Answer:**
A class declared using the `abstract` keyword that cannot be instantiated.

---

## 20. Can we create an object of an Abstract Class?

**Answer:**
No.

---

## 21. What is an Interface?

**Answer:**
An interface is a blueprint that contains method declarations and is implemented by classes.

---

## 22. Difference between Interface and Abstract Class?

| Interface                     | Abstract Class          |
| ----------------------------- | ----------------------- |
| Uses implements               | Uses extends            |
| Supports Multiple Inheritance | Does Not                |
| Methods mostly abstract       | Can have normal methods |

---

## 23. What is a Constructor?

**Answer:**
A special method used to initialize objects.

---

## 24. Can a Constructor be Overloaded?

**Answer:**
Yes.

---

## 25. Can a Constructor be Overridden?

**Answer:**
No.

---

## 26. What is the purpose of the `this` keyword?

**Answer:**
It refers to the current object of the class.

---

## 27. What is the purpose of the `super` keyword?

**Answer:**
It refers to the parent class object and members.

---

## 28. What is Association?

**Answer:**
A relationship between two independent classes.

Example: Teacher and Student.

---

## 29. What is Aggregation?

**Answer:**
A weak HAS-A relationship where the child object can exist independently.

Example: Student HAS-A Address.

---

## 30. What is Composition?

**Answer:**
A strong HAS-A relationship where the child object cannot exist independently.

Example: Car HAS-A Engine.

---

## 31. What is the Diamond Problem?

**Answer:**
An ambiguity that occurs when a class inherits from two classes having the same method. Java avoids this by not supporting multiple inheritance through classes.

---

## 32. Can an Interface extend another Interface?

**Answer:**
Yes.

---

## 33. Can a Class implement multiple Interfaces?

**Answer:**
Yes.

```java
class A implements X, Y {
}
```

---

## 34. Can an Abstract Class have Constructors?

**Answer:**
Yes.

---

## 35. Which OOPS concept provides Security?

**Answer:**
Encapsulation.

---

## 36. Which OOPS concept provides Code Reusability?

**Answer:**
Inheritance.

---

## 37. Which OOPS concept provides Flexibility?

**Answer:**
Polymorphism.

---

## 38. Which OOPS concept hides complexity?

**Answer:**
Abstraction.

---

## 39. What is Dynamic Binding?

**Answer:**
The method call is resolved during runtime. It occurs in Method Overriding.

---

## 40. What is Static Binding?

**Answer:**
The method call is resolved during compile time. It occurs in Method Overloading.

---

## 41. Is Java 100% Object-Oriented?

**Answer:**
No. Java uses primitive data types (`int`, `char`, `float`, etc.), so it is not 100% object-oriented.

---

## 42. What is Runtime Polymorphism?

**Answer:**
Method execution is decided at runtime based on the object created.

---

## 43. What is Compile-Time Polymorphism?

**Answer:**
Method execution is decided during compilation based on method signatures.

---

## 44. What is a HAS-A Relationship?

**Answer:**
A relationship where one class contains another class object.

Example: Car HAS-A Engine.

---

## 45. What is an IS-A Relationship?

**Answer:**
Inheritance relationship.

Example: Dog IS-A Animal.

---

## 46. Can we instantiate an Interface?

**Answer:**
No.

---

## 47. Which keyword is used for Inheritance?

**Answer:**

```java
extends
```

---

## 48. Which keyword is used to implement an Interface?

**Answer:**

```java
implements
```

---

## 49. Which keyword is used to create an Abstract Class?

**Answer:**

```java
abstract
```

---

## 50. Which OOPS topic is asked most in Java interviews?

**Answer:**

1. Encapsulation
2. Inheritance
3. Method Overloading
4. Method Overriding
5. Interface vs Abstract Class
6. `this` vs `super`
7. Association vs Aggregation vs Composition
8. Constructor concepts
9. Runtime Polymorphism
10. Diamond Problem

These 50 questions cover the most frequently asked OOPS interview, viva, and placement questions in Java.
