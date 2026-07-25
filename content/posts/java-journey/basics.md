---
date: 2026-07-25T01:00:31+03:00
title: Basics
categories:
  - Java
tags:
  - oop
  - basics
series:
  - Java Journey
series_order: 1
---
## Java Overview

Java is a General-Purpose, Object-Oriented Programming Language that is guaranteed to be Write Once, Run Anywhere and is used in Android apps, banking, enterprise systems, and more.

## Principles of Object-Oriented Programming (OOP)

* **Encapsulation**: Keeping data safe inside classes
* **Abstraction**: Hiding complex logic behind simple interfaces
* **Inheritance**: Reusing code through parent-child relationships
* **Polymorphism**: One method, many forms (for example method overriding)

## Classes vs Objects

| Class                                           | Object                                              |
| ----------------------------------------------- | --------------------------------------------------- |
| Blueprint of an object; used to create objects  | Instance of a class                                 |
| No memory is allocated when a class is declared | Memory is allocated as soon as an object is created |
| Logical entity                                  | Physical entity                                     |
| Group of similar objects                        | Real-world entity, such as a book or a car          |
| Can only be declared once                       | Can be created many times as per the requirement    |
| Example: `Car`                                  | Examples: `BMW, Mercedes, Ferrari`                  |

## Errors vs Exceptions

| Error | Exception |
|---|---|
| Indicates a serious problem that a reasonable application should not try to catch | Indicates conditions that a reasonable application might try to catch |
| Caused by issues with the JVM or hardware | Caused by conditions in the program, such as invalid input or logic errors |
| Examples: `OutOfMemoryError`, `StackOverflowError` | Examples: `IOException`, `NullPointerException` |

## Best Practices in Java

1. Use meaningful variable and method names
2. Keep methods short and focused
3. Favor composition over inheritance
4. Handle exceptions properly  - don't swallow them silently
5. Avoid using `null` - prefer `Optional`
6. Stick to consistent coding conventions (indentation, naming)
7. Use `final` where possible to make code more predictable
8. Write unit tests alongside your code, not after - they catch regressions early
9. Prefer immutability where practical - fewer moving parts means fewer bugs
