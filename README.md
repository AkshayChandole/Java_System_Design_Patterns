
# Java System Design Patterns

Welcome to the Java System Design Patterns repository! This repository contains examples and explanations of various design patterns in Java.

## Table of Contents

1. [Introduction](#repo-introduction)
   - [About this Repository](#about-this-repository)
   - [How to Use this Repository](#how-to-use-this-repository)

2. [Introduction to design patterns](#design-patterns-introduction)
   - [What are design patterns?](#what-are-design-patterns)	
   - [Advantages of design patterns](#advantages-of-design-pattern)
   - [Consequences of unfamiliarity with the design patterns](#consequences-of-unfamilarity-with-the-design-patterns)
   - [Classification of design patterns](#classification-of-design-pattern)
     
3. [Creational Patterns](#creational-patterns)
   - [Singleton Pattern](#singleton-pattern)
   - [Factory Method Pattern](#factory-method-pattern)
   - [Abstract Factory Pattern](#abstract-factory-pattern)
   - [Builder Pattern](#builder-pattern)
   - [Prototype Pattern](#prototype-pattern)
   - [Constructor Pattern](#constructor-pattern)

4. [Structural Patterns](#structural-patterns)
   - [Adapter Pattern](#adapter-pattern)
   - [Bridge Pattern](#bridge-pattern)
   - [Composite Pattern](#composite-pattern)
   - [Decorator Pattern](#decorator-pattern)
   - [Facade Pattern](#facade-pattern)
   - [Flyweight Pattern](#flyweight-pattern)
   - [Proxy Pattern](#proxy-pattern)

5. [Behavioral Patterns](#behavioral-patterns)
   - [Chain of Responsibility Pattern](#chain-of-responsibility-pattern)
   - [Command Pattern](#command-pattern)
   - [Interpreter Pattern](#interpreter-pattern)
   - [Iterator Pattern](#iterator-pattern)
   - [Mediator Pattern](#mediator-pattern)
   - [Memento Pattern](#memento-pattern)
   - [Observer Pattern](#observer-pattern)
   - [State Pattern](#state-pattern)
   - [Strategy Pattern](#strategy-pattern)
   - [Template Method Pattern](#template-method-pattern)
   - [Visitor Pattern](#visitor-pattern)

6. [Concurrency Patterns](#concurrency-patterns)
   - [Thread Pool Pattern](#thread-pool-pattern)
   - [Thread-Safe Singleton Pattern](#thread-safe-singleton-pattern)
   - [Producer-Consumer Pattern](#producer-consumer-pattern)
   - [Read-Write Lock Pattern](#read-write-lock-pattern)
   - [Fork/Join Pattern](#forkjoin-pattern)

7. [Architectural Patterns](#architectural-patterns)
   - [MVC Pattern](#mvc-pattern)   
   - [MVP Pattern](#mvp-pattern)
   - [MVVM Pattern](#mvvm-pattern)
   - [DAO Pattern](#dao-pattern)
   - [Service Locator Pattern](#service-locator-pattern)
   - [Dependency Injection Pattern](#dependency-injection-pattern)

8. [Contributing](#contributing)
  - [How to Contribute](#how-to-contribute)
  - [License](#license)
 
 <hr>  
 
## Introduction

### About this Repository

This repository aims to provide a comprehensive guide to various design patterns in Java. Each pattern includes a detailed explanation, code examples, and real-world use cases.

### How to Use this Repository

Browse through the different sections to learn about various design patterns. Each pattern is explained with examples and use cases to help you understand how to implement it in your projects.

<br>

## Introduction to Design Patterns

### What are Design Patterns?

Design patterns are proven solutions to common problems in software design. They represent best practices that the experienced object-oriented software developers have used over time. Design patterns provide a template for writing software that is flexible, reusable, and adaptable to changes.

### Advantages of Design Patterns

1.  **Reusability**: Design patterns provide a proven solution to common problems, allowing developers to reuse successful strategies across different projects.
2.  **Efficiency**: Using design patterns can save time by providing ready-made solutions, thereby reducing the need to reinvent the wheel.
3.  **Maintainability**: Code that follows design patterns is generally more understandable and easier to maintain. This results in better collaboration among team members and makes it easier to manage changes.
4.  **Scalability**: Design patterns help in writing scalable code that can grow and adapt to changing requirements.
5.  **Standardization**: Design patterns provide a common vocabulary for designers, leading to clearer communication and better understanding among developers.

### Consequences of Unfamiliarity with Design Patterns

1.  **Reinventing the Wheel**: Developers may end up creating inefficient solutions for problems that have already been solved, leading to wasted time and effort.
2.  **Inconsistency**: Without design patterns, code may lack consistency, making it harder to understand, maintain, and extend.
3.  **Poor Quality Code**: The absence of design patterns can lead to poor code quality, with issues such as tight coupling, lack of modularity, and difficulty in managing changes.
4.  **Increased Bugs**: Not following established patterns can introduce bugs and vulnerabilities, as the code might not follow best practices for robustness and security.

### Classification of Design Patterns
![classification](https://github.com/user-attachments/assets/b46be479-f6f8-4cc6-8f15-33e606f45fde)

Design patterns can be classified into several categories based on their purpose and scope. The primary categories include:

1.  **Creational Patterns**: Deal with object creation mechanisms, trying to create objects in a manner suitable to the situation. Examples include Singleton, Factory Method, and Builder patterns.
2.  **Structural Patterns**: Concerned with how classes and objects are composed to form larger structures. Examples include Adapter, Composite, and Proxy patterns.
3.  **Behavioral Patterns**: Deal with algorithms and the assignment of responsibilities between objects. Examples include Observer, Strategy, and Command patterns.
4.  **Concurrency Patterns**: Address multi-threaded programming paradigms. Examples include Thread Pool, Producer-Consumer, and Read-Write Lock patterns.
5.  **Architectural Patterns**: Deal with the overall architecture of an application. Examples include MVC (Model-View-Controller), MVP (Model-View-Presenter), and MVVM (Model-View-ViewModel) patterns.

Understanding and applying design patterns is crucial for developing robust, maintainable, and scalable software. This repository aims to provide a comprehensive guide to various design patterns in Java, helping you incorporate these best practices into your projects.


<br>

## Contributing

### How to Contribute

Fork the repository, make your changes, and submit a pull request. 


### License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/AkshayChandole/Java_System_Design_Patterns/blob/main/LICENSE) file for details.
