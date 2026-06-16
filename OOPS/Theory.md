# OOPS (Object-Oriented Programming System) in Java – Theory

## What is OOPS?

OOPS (Object-Oriented Programming System) is a programming paradigm that organizes software around **objects** rather than functions and logic.

An object contains:

* **Data (Attributes/Variables)**
* **Behavior (Methods/Functions)**

Java is primarily an Object-Oriented Programming language.

### Advantages of OOPS

* Code Reusability
* Better Security
* Easy Maintenance
* Modularity
* Scalability
* Real-world Modeling

---

# Basic OOPS Terminologies

## 1. Class

A class is a blueprint or template used to create objects.

### Definition

A class defines:

* Data members (variables)
* Methods (functions)

Example:

* Car is a class.
* It defines color, model, speed, etc.

---

## 2. Object

An object is an instance of a class.

### Characteristics

* Has State (data)
* Has Behavior (methods)
* Occupies Memory

Example:

* BMW Car
* Audi Car

Both are objects of the Car class.

---

## 3. Method

A method is a block of code that performs a specific task.

### Purpose

* Defines behavior of objects.
* Improves code reusability.

---

## 4. Constructor

A constructor is a special method used to initialize objects.

### Characteristics

* Same name as class name.
* No return type.
* Automatically called when an object is created.

---

# Four Pillars of OOPS

---

# 1. Encapsulation

## Definition

Encapsulation is the process of wrapping data and methods into a single unit (class).

It hides internal details from outside users.

### Purpose

* Data Security
* Controlled Access
* Better Maintenance

### Features

* Variables are usually declared private.
* Access provided through methods.

### Real-Life Example

ATM Machine:

* User enters PIN.
* Internal process is hidden.

---

# 2. Inheritance

## Definition

Inheritance is the process by which one class acquires properties and behaviors of another class.

### Purpose

* Code Reusability
* Reduces Redundancy
* Easier Maintenance

### Types of Inheritance in Java

### Single Inheritance

One child inherits one parent.

### Multilevel Inheritance

Grandparent → Parent → Child

### Hierarchical Inheritance

One parent → Multiple children

### Multiple Inheritance

Not supported through classes in Java.
Supported using interfaces.

### Hybrid Inheritance

Combination of inheritance types using interfaces.

### Real-Life Example

Animal → Dog

Dog inherits properties of Animal.

---

# 3. Polymorphism

## Definition

Polymorphism means "Many Forms".

The same method can perform different actions depending on the situation.

### Advantages

* Flexibility
* Reusability
* Easy Extension

### Types of Polymorphism

### Compile-Time Polymorphism

Also called:

* Method Overloading
* Static Binding

Decision made during compilation.

### Runtime Polymorphism

Also called:

* Method Overriding
* Dynamic Binding

Decision made during execution.

### Real-Life Example

A person can be:

* Student
* Employee
* Customer

Same person, different roles.

---

# 4. Abstraction

## Definition

Abstraction is the process of hiding implementation details and showing only essential features.

### Purpose

* Reduces Complexity
* Improves Security
* Focuses on Important Information

### Achieved Through

* Abstract Classes
* Interfaces

### Real-Life Example

Car Driving:

* Driver uses steering, brake, accelerator.
* Internal engine mechanism is hidden.

---

# Additional OOPS Concepts

## Association

A relationship between two independent classes.

### Example

Teacher and Student

Both can exist independently.

---

## Aggregation

A special form of Association.

### Definition

One class contains another class.

### Characteristics

* Weak Relationship
* Child can exist independently.

### Example

Department and Teacher

Teacher can exist without Department.

---

## Composition

A strong form of Aggregation.

### Characteristics

* Strong Relationship
* Child cannot exist without Parent.

### Example

House and Room

If House is destroyed, Rooms also cease to exist.

---

## Interface

### Definition

An interface is a blueprint containing method declarations.

### Features

* Supports Multiple Inheritance.
* Achieves 100% Abstraction (conceptually).
* Methods are implemented by classes.

---

## Abstract Class

### Definition

A class declared using the abstract keyword.

### Features

* Can contain abstract methods.
* Can contain normal methods.
* Cannot be instantiated.

---

# Difference Between Class and Object

| Class                  | Object             |
| ---------------------- | ------------------ |
| Blueprint              | Instance           |
| Logical Entity         | Physical Entity    |
| No Memory Allocation   | Memory Allocated   |
| Used to Create Objects | Created from Class |

---

# Difference Between Interface and Abstract Class

| Interface                     | Abstract Class            |
| ----------------------------- | ------------------------- |
| Supports Multiple Inheritance | Does Not                  |
| Methods Mostly Abstract       | Can Have Both             |
| Variables are Constants       | Can Have Normal Variables |
| Uses implements               | Uses extends              |

---

# Difference Between Encapsulation and Abstraction

| Encapsulation                   | Abstraction                             |
| ------------------------------- | --------------------------------------- |
| Hides Data                      | Hides Implementation                    |
| Achieved Using Access Modifiers | Achieved Using Abstract Class/Interface |
| Focuses on Security             | Focuses on Simplicity                   |

---

# OOPS Principles Summary

1. **Class** → Blueprint of objects.
2. **Object** → Instance of a class.
3. **Encapsulation** → Data Hiding.
4. **Inheritance** → Code Reusability.
5. **Polymorphism** → One Interface, Many Forms.
6. **Abstraction** → Hiding Implementation Details.
7. **Association** → Relationship Between Classes.
8. **Aggregation** → Weak HAS-A Relationship.
9. **Composition** → Strong HAS-A Relationship.
10. **Interface** → Multiple Inheritance & Abstraction.
11. **Abstract Class** → Partial Abstraction.

These are the complete theory concepts of OOPS in Java commonly asked in interviews, viva exams, and placement assessments.
