# OOPS in Java – Clear Examples Only

## 1. Class

```java
class Student {
    String name;
}
```

`Student` is a class.

---

## 2. Object

```java
class Student {
    String name;
}

public class Main {
    public static void main(String[] args) {
        Student s1 = new Student();
    }
}
```

`s1` is an object of the `Student` class.

---

## 3. Method

```java
class Student {
    void study() {
        System.out.println("Studying...");
    }
}
```

`study()` is a method.

---

## 4. Constructor

```java
class Student {
    Student() {
        System.out.println("Constructor Called");
    }
}
```

Constructor executes automatically when an object is created.

---

# Encapsulation

```java
class Student {
    private int age;

    public void setAge(int age) {
        this.age = age;
    }

    public int getAge() {
        return age;
    }
}
```

Data is hidden using `private` and accessed through methods.

---

# Inheritance

```java
class Animal {
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Barking");
    }
}
```

`Dog` inherits `eat()` from `Animal`.

---

# Single Inheritance

```java
class A {
    void show() {
        System.out.println("Class A");
    }
}

class B extends A {
}
```

One parent → One child.

---

# Multilevel Inheritance

```java
class A {
    void showA() {
        System.out.println("A");
    }
}

class B extends A {
    void showB() {
        System.out.println("B");
    }
}

class C extends B {
    void showC() {
        System.out.println("C");
    }
}
```

A → B → C

---

# Hierarchical Inheritance

```java
class Animal {
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal {
}

class Cat extends Animal {
}
```

One parent → Multiple children.

---

# Polymorphism

## Method Overloading (Compile Time)

```java
class Maths {
    void add(int a, int b) {
        System.out.println(a + b);
    }

    void add(int a, int b, int c) {
        System.out.println(a + b + c);
    }
}
```

Same method name, different parameters.

---

## Method Overriding (Runtime)

```java
class Animal {
    void sound() {
        System.out.println("Animal Sound");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Bark");
    }
}
```

Child class changes parent method behavior.

---

# Abstraction

## Abstract Class

```java
abstract class Animal {
    abstract void sound();
}

class Dog extends Animal {
    void sound() {
        System.out.println("Bark");
    }
}
```

Only important functionality is shown.

---

# Interface

```java
interface Animal {
    void sound();
}

class Dog implements Animal {
    public void sound() {
        System.out.println("Bark");
    }
}
```

Interface methods are implemented by classes.

---

# Association

```java
class Teacher {
}

class Student {
    Teacher t;
}
```

Teacher and Student are associated.

---

# Aggregation

```java
class Address {
    String city;
}

class Student {
    Address address;
}
```

Student HAS-A Address.

Address can exist independently.

---

# Composition

```java
class Engine {
}

class Car {
    private Engine engine = new Engine();
}
```

Car strongly owns Engine.

Engine depends on Car.

---

# this Keyword

```java
class Student {
    String name;

    Student(String name) {
        this.name = name;
    }
}
```

`this` refers to the current object.

---

# super Keyword

```java
class Animal {
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal {
    void display() {
        super.eat();
    }
}
```

`super` accesses parent class members.

---

# Object Creation Example

```java
class Car {
    String brand = "BMW";

    void display() {
        System.out.println(brand);
    }
}

public class Main {
    public static void main(String[] args) {
        Car c1 = new Car();
        c1.display();
    }
}
```

Output:

```
BMW
```

---

# Real OOPS Example

```java
class Employee {
    String name;

    Employee(String name) {
        this.name = name;
    }

    void work() {
        System.out.println(name + " is working");
    }
}

public class Main {
    public static void main(String[] args) {
        Employee e1 = new Employee("Sujan");
        e1.work();
    }
}
```

Output:

```
Sujan is working
```


