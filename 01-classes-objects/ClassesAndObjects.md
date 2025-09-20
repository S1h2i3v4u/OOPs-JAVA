# Classes and Objects in Java

## 1. Introduction

Java is an Object-Oriented Programming Language (OOP).

- Class → Blueprint/template to create objects.
- Object → Instance of a class (real-world entity).

👉 Example:

- Class = Car (blueprint)
- Objects = Honda, BMW, Tesla

## 2. What is a Class?

A class in Java is a user-defined data type that acts as a blueprint for objects.

Syntax:
```
class ClassName {
    // Fields (variables / attributes)
    // Methods (functions / behaviors)
}
```

Example:
```
class Car {
    // Fields
    String brand;
    int speed;

    // Method
    void drive() {
        System.out.println(brand + " is driving at " + speed + " km/h");
    }
}

```

## 3. What is an Object?

An object is an instance of a class, created using the new keyword.

Syntax:
```
ClassName obj = new ClassName();

```

Example:
```
public class Main {
    public static void main(String[] args) {
        // Creating object
        Car car1 = new Car();
        car1.brand = "BMW";
        car1.speed = 120;
        car1.drive();

        Car car2 = new Car();
        car2.brand = "Tesla";
        car2.speed = 150;
        car2.drive();
    }
}

```
Output:
```
BMW is driving at 120 km/h
Tesla is driving at 150 km/h

```

## 4. Memory Allocation

When an object is created:

- Fields (variables) → Stored in heap memory.

- Reference variable → Stored in stack memory.

👉 Example:
```
Car car1 = new Car();

```
- car1 (reference) → Stack
- new Car() (object) → Heap

## 5. Multiple Objects

- You can create multiple objects from the same class.
- Each object has its own copy of instance variables.

```
Car car1 = new Car();
Car car2 = new Car();
```

## 6. Anonymous Objects

Objects without a reference variable. Used only once.
```
new Car().drive();
```
## 7. Class Members

- Instance variables → Belong to objects
- Static variables → Belong to class (shared)
- Methods → Define behavior
- Constructors → Initialize objects

## 8. Key Points

- A class is a logical entity, not memory-allocated until objects are created.
- An object is a physical entity (created at runtime).
- A class can have multiple objects.
- Objects are created using 'new' keyword.
