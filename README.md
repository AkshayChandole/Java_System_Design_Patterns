
# Java System Design Patterns

Welcome to the Java System Design Patterns repository! This repository contains examples and explanations of various design patterns in Java.

## Table of Contents

1. [Introduction](#introduction)
   - [About this Repository](#about-this-repository)
   - [How to Use this Repository](#how-to-use-this-repository)

2. [Introduction to Design Patterns](#design-patterns-introduction)
   - [What are Design Patterns?](#what-are-design-patterns)	
   - [Advantages of Design Patterns](#advantages-of-design-pattern)
   - [Consequences of Unfamiliarity with Design Patterns](#consequences-of-unfamiliarity-with-design-patterns)
   - [Classification of Design Patterns](#classification-of-design-patterns)
     
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


<hr>

## Creational Patterns

Creational patterns provide various object creation mechanisms, which increase flexibility and reuse of existing code. These patterns deal with the process of object creation in a manner suitable to the situation at hand. They abstract the instantiation process and make it more adaptable to change, ensuring that the system remains flexible and scalable.

### Purpose of Creational Patterns

1. **Encapsulation of Object Creation Logic**: By abstracting the instantiation process, these patterns encapsulate the logic that determines which type of object to create under varying conditions.
2. **Flexibility**: They promote loose coupling by reducing the dependency between the client code and the classes that instantiate objects. This makes the system more adaptable to changes.
3. **Reusability**: By reusing existing objects and sharing them appropriately, creational patterns help in efficient memory management and enhance the reusability of code.

### Common Characteristics

- **Object Creation**: These patterns focus on the best ways to instantiate and configure objects.
- **Encapsulation**: They encapsulate the knowledge about which concrete classes are used by hiding the specifics behind interfaces or abstract classes.
- **Abstraction**: They promote the use of abstract classes or interfaces to define the creation steps without specifying the exact class of objects to be created.

### Benefits

- **Improved Flexibility**: They allow a system to be configured with "plug-in" components, promoting higher flexibility.
- **Enhanced Reusability**: By defining standard ways to create objects, these patterns enable reusability of the object creation code.
- **Easier Maintenance**: Changes in the creation logic are localized, making the system easier to maintain and extend.

### When to Use

- **When the exact type and dependencies of objects are not known until runtime**: Creational patterns are beneficial when the system should be independent of how its objects are created, composed, and represented.
- **When constructing an object involves complex creation logic**: They simplify the object creation process and manage the complexity by encapsulating the creation logic.
- **When managing and controlling a group of related objects**: They provide a way to manage and control the lifecycle of objects within a particular group.

Creational patterns play a crucial role in ensuring that a system is well-designed and flexible, enabling easier maintenance and scalability. In the following sections, we will explore different creational patterns, their implementations, and real-world use cases to help you understand their importance and application in software design.

---


### Singleton Pattern

The Singleton Pattern is one of the simplest and most commonly used design patterns in software development. It ensures that a class has only one instance and provides a global point of access to that instance.

#### Introduction

The Singleton Pattern restricts the instantiation of a class to a single instance. This is useful when exactly one object is needed to coordinate actions across the system. The pattern involves a single class that is responsible for creating an object while making sure that only one object gets created.

![Singleton Pattern](https://github.com/user-attachments/assets/02ab6b55-882f-440f-a6c6-06d07d9e970a)

#### Problem it Solves

In certain scenarios, it is important to have exactly one instance of a class. Examples include:

-   **Configuration settings**: Ensuring there is a single source of truth for configuration data.
-   **Logging**: Ensuring all parts of an application log messages to a single logger instance.
-   **Connection Pools**: Managing a pool of database connections through a single manager object.

Without the Singleton Pattern, multiple instances of these classes could be created, leading to inconsistent behavior, resource contention, or performance issues.

#### How to Implement the Singleton Pattern

In Java, the Singleton Pattern can be implemented using several approaches. The most common implementations are:

1.  **Eager Initialization**: The instance of the class is created at the time of class loading.
2.  **Lazy Initialization**: The instance is created only when it is requested for the first time.
3.  **Thread-safe Singleton**: Ensures that the instance is created in a thread-safe manner.
4.  **Bill Pugh Singleton**: Uses an inner static helper class for initialization, which ensures thread-safety and lazy initialization.

##### Example: Eager Initialization

```java
// EagerSingleton.java 

public class EagerSingleton {

    // Create the instance at the time of class loading
    private static final EagerSingleton instance = new EagerSingleton();

    // Private constructor to restrict instantiation of the class from other classes
    private EagerSingleton() {}

    // Public method to provide access to the instance
    public static EagerSingleton getInstance() {
        return instance;
    }

    // Method to demonstrate singleton behavior
    public void showMessage() {
        System.out.println("Hello World! This is an Eager Initialization Singleton pattern example.");
    }
}
```

##### Example: Lazy Initialization

```java
// Singleton.java

public class Singleton {

    // Private static variable of the same class that is the only instance of the class.
    private static Singleton instance;

    // Private constructor to restrict instantiation of the class from other classes.
    private Singleton() {}

    // Public static method that returns the instance of the class, this is the global access point for the outer world to get the instance of the singleton class.
    public static Singleton getInstance() {
        if (instance == null) {
            instance = new Singleton();
        }
        return instance;
    }

    // Method to demonstrate singleton behavior
    public void showMessage() {
        System.out.println("Hello World! This is a Singleton pattern example.");
    }
}
```

##### Example: Thread-safe Singleton

``` java
// ThreadSafeSingleton.java

public class ThreadSafeSingleton {

    // The field must be declared volatile so that double check lock would work correctly.
    private static volatile ThreadSafeSingleton instance;

    // Private constructor to restrict instantiation of the class from other classes.
    private ThreadSafeSingleton() {}

    public static synchronized ThreadSafeSingleton getInstance() {
	    // The approach taken here is called double-checked locking (DCL).
        // It exists to prevent race condition between multiple threads that may
        // attempt to get singleton instance at the same time, creating separate
        // instances as a result.
        ThreadSafeSingleton result = instance;
        if (result != null) {
            return result;
        }
        synchronized(ThreadSafeSingleton.class) {
            if (instance == null) {
                instance = new ThreadSafeSingleton(value);
            }
            return instance;
        }
    }

    // Method to demonstrate singleton behavior
    public void showMessage() {
        System.out.println("Hello World! This is a Thread-safe Singleton pattern example.");
    }
}
```

##### Example: Bill Pugh Singleton

```java
public class BillPughSingleton {

    // Private constructor to restrict instantiation of the class from other classes.
    private BillPughSingleton() {}

    // Static inner class - inner classes are not loaded until they are referenced.
    private static class SingletonHelper {
        // Inner class is referenced after getInstance() is called
        private static final BillPughSingleton INSTANCE = new BillPughSingleton();
    }

    // Global access point for outer world to get the instance of the singleton class.
    public static BillPughSingleton getInstance() {
        return SingletonHelper.INSTANCE;
    }

    // Method to demonstrate singleton behavior
    public void showMessage() {
        System.out.println("Hello World! This is a Bill Pugh Singleton pattern example.");
    }
}
```

#### Pros

1.  **Controlled Access to the Single Instance**: It provides a controlled access point for the unique instance.
2.  **Reduced Namespace Pollution**: It avoids unnecessary duplication of objects.
3.  **Flexibility**: Singleton patterns can be extended to support a variable number of instances.
4.  **Consistent Data**: Ensures that a single instance holds all the necessary state and data, leading to consistent behavior across the application.

#### Cons

1.  **Difficulty in Testing**: Singleton classes can be difficult to unit test because they carry state and often use global access points.
2.  **Hidden Dependencies**: Singleton can introduce hidden dependencies into a system as it provides a global point of access.
3.  **Concurrency Issues**: If not implemented correctly, Singleton can lead to issues in a multithreaded environment.
4.  **Global State**: Singleton can encourage the use of global state, which can make the system harder to understand and maintain.

#### Real-Life Example: Database Connection Manager

In many applications, managing database connections is critical. The Database Connection Manager should ensure that only one connection pool exists throughout the application to manage database connections efficiently.

##### DatabaseConnectionManager.java

```java
// DatabaseConnectionManager.java

public class DatabaseConnectionManager {

    private static DatabaseConnectionManager instance;
    private Connection connection;
    private String url = "jdbc:mysql://localhost:3306/mydatabase";
    private String username = "root";
    private String password = "password";

    private DatabaseConnectionManager() throws SQLException {
        try {
            Class.forName("com.mysql.cj.jdbc.Driver");
            this.connection = DriverManager.getConnection(url, username, password);
        } catch (ClassNotFoundException | SQLException ex) {
            throw new RuntimeException("Error connecting to the database", ex);
        }
    }

    public static DatabaseConnectionManager getInstance() throws SQLException {
        if (instance == null) {
            instance = new DatabaseConnectionManager();
        } else if (instance.getConnection().isClosed()) {
            instance = new DatabaseConnectionManager();
        }
        return instance;
    }

    public Connection getConnection() {
        return connection;
    }
}
```

##### Usage Example

```java
// Main.class

public class Main {
    public static void main(String[] args) {
        try {
            DatabaseConnectionManager connectionManager = DatabaseConnectionManager.getInstance();
            Connection connection = connectionManager.getConnection();
            // Use the connection for database operations
            System.out.println("Database connection established successfully!");

        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
```

In this example, the `DatabaseConnectionManager` class ensures that there is only one instance managing the database connections. This singleton instance can be used throughout the application to get the database connection, ensuring efficient use of resources and consistent behavior.



<hr>
## Contributing

### How to Contribute

Fork the repository, make your changes, and submit a pull request. 


### License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/AkshayChandole/Java_System_Design_Patterns/blob/main/LICENSE) file for details.
