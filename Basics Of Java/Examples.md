
# 1. Variables

```java
public class Main {
    public static void main(String[] args) {
        int age = 20;
        double salary = 25000.50;
        char grade = 'A';
        boolean pass = true;

        System.out.println(age);
        System.out.println(salary);
        System.out.println(grade);
        System.out.println(pass);
    }
}
```

---

# 2. Arithmetic Operators

```java
public class Main {
    public static void main(String[] args) {
        int a = 10, b = 5;

        System.out.println(a + b); // 15
        System.out.println(a - b); // 5
        System.out.println(a * b); // 50
        System.out.println(a / b); // 2
        System.out.println(a % b); // 0
    }
}
```

---

# 3. Relational Operators

```java
public class Main {
    public static void main(String[] args) {
        int a = 10, b = 20;

        System.out.println(a > b);
        System.out.println(a < b);
        System.out.println(a == b);
        System.out.println(a != b);
    }
}
```

---

# 4. Logical Operators

```java
public class Main {
    public static void main(String[] args) {
        int age = 20;

        System.out.println(age > 18 && age < 30);
        System.out.println(age > 25 || age < 30);
        System.out.println(!(age > 18));
    }
}
```

---

# 5. If Statement

```java
public class Main {
    public static void main(String[] args) {
        int age = 18;

        if(age >= 18){
            System.out.println("Eligible to Vote");
        }
    }
}
```

---

# 6. If-Else

```java
public class Main {
    public static void main(String[] args) {
        int marks = 40;

        if(marks >= 35){
            System.out.println("Pass");
        } else {
            System.out.println("Fail");
        }
    }
}
```

---

# 7. Else If Ladder

```java
public class Main {
    public static void main(String[] args) {
        int marks = 85;

        if(marks >= 90){
            System.out.println("Grade A");
        }
        else if(marks >= 75){
            System.out.println("Grade B");
        }
        else{
            System.out.println("Grade C");
        }
    }
}
```

---

# 8. Switch Statement

```java
public class Main {
    public static void main(String[] args) {
        int day = 2;

        switch(day){
            case 1:
                System.out.println("Monday");
                break;
            case 2:
                System.out.println("Tuesday");
                break;
            default:
                System.out.println("Invalid Day");
        }
    }
}
```

---

# 9. For Loop

```java
public class Main {
    public static void main(String[] args) {

        for(int i=1;i<=5;i++){
            System.out.println(i);
        }

    }
}
```

Output:

```
1
2
3
4
5
```

---

# 10. While Loop

```java
public class Main {
    public static void main(String[] args) {

        int i=1;

        while(i<=5){
            System.out.println(i);
            i++;
        }

    }
}
```

---

# 11. Do While Loop

```java
public class Main {
    public static void main(String[] args) {

        int i=1;

        do{
            System.out.println(i);
            i++;
        }while(i<=5);

    }
}
```

---

# 12. Break

```java
public class Main {
    public static void main(String[] args) {

        for(int i=1;i<=10;i++){

            if(i==5)
                break;

            System.out.println(i);
        }
    }
}
```

Output:

```
1
2
3
4
```

---

# 13. Continue

```java
public class Main {
    public static void main(String[] args) {

        for(int i=1;i<=5;i++){

            if(i==3)
                continue;

            System.out.println(i);
        }
    }
}
```

Output:

```
1
2
4
5
```

---

# 14. Array

```java
public class Main {
    public static void main(String[] args) {

        int arr[] = {10,20,30,40,50};

        for(int i=0;i<arr.length;i++){
            System.out.println(arr[i]);
        }
    }
}
```

---

# 15. Enhanced For Loop

```java
public class Main {
    public static void main(String[] args) {

        int arr[] = {10,20,30};

        for(int num : arr){
            System.out.println(num);
        }
    }
}
```

---

# 16. String

```java
public class Main {
    public static void main(String[] args) {

        String name = "Sujan";

        System.out.println(name);
        System.out.println(name.length());
    }
}
```

---

# 17. String Methods

```java
public class Main {
    public static void main(String[] args) {

        String str = "Java Programming";

        System.out.println(str.toUpperCase());
        System.out.println(str.toLowerCase());
        System.out.println(str.charAt(2));
        System.out.println(str.contains("Java"));
    }
}
```

---

# 18. Method (Function)

```java
public class Main {

    static void greet(){
        System.out.println("Hello");
    }

    public static void main(String[] args) {
        greet();
    }
}
```

---

# 19. Method with Parameters

```java
public class Main {

    static void add(int a,int b){
        System.out.println(a+b);
    }

    public static void main(String[] args) {
        add(10,20);
    }
}
```

---

# 20. Class and Object

```java
class Student{

    String name = "Sujan";

    void display(){
        System.out.println(name);
    }
}

public class Main {
    public static void main(String[] args) {

        Student s = new Student();
        s.display();

    }
}
```

---

# 21. Inheritance

```java
class Animal{
    void sound(){
        System.out.println("Animal Sound");
    }
}

class Dog extends Animal{
}

public class Main {
    public static void main(String[] args) {

        Dog d = new Dog();
        d.sound();

    }
}
```

---

# 22. Exception Handling

```java
public class Main {
    public static void main(String[] args) {

        try{
            int a = 10/0;
        }
        catch(Exception e){
            System.out.println("Error Handled");
        }

    }
}
```

---

# 23. Multithreading

```java
class MyThread extends Thread{

    public void run(){
        System.out.println("Thread Running");
    }
}

public class Main {
    public static void main(String[] args) {

        MyThread t = new MyThread();
        t.start();

    }
}
```

These are the most commonly asked Java basics examples for interviews, lab exams, viva, and placement training. 🚀
