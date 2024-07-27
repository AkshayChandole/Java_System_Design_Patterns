
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


## Singleton Pattern

The Singleton Pattern is one of the simplest and most commonly used design patterns in software development. It ensures that a class has only one instance and provides a global point of access to that instance.

### Introduction

The Singleton Pattern restricts the instantiation of a class to a single instance. This is useful when exactly one object is needed to coordinate actions across the system. The pattern involves a single class that is responsible for creating an object while making sure that only one object gets created.

![Singleton Pattern](https://github.com/user-attachments/assets/c847232a-1f1e-4dcd-a20c-c8382f092aeb)


### Problem it Solves

In certain scenarios, it is important to have exactly one instance of a class. Examples include:

-   **Configuration settings**: Ensuring there is a single source of truth for configuration data.
-   **Logging**: Ensuring all parts of an application log messages to a single logger instance.
-   **Connection Pools**: Managing a pool of database connections through a single manager object.

Without the Singleton Pattern, multiple instances of these classes could be created, leading to inconsistent behavior, resource contention, or performance issues.

### How to Implement the Singleton Pattern

In Java, the Singleton Pattern can be implemented using several approaches. The most common implementations are:

1.  **Eager Initialization**: The instance of the class is created at the time of class loading.
2.  **Lazy Initialization**: The instance is created only when it is requested for the first time.
3.  **Thread-safe Singleton**: Ensures that the instance is created in a thread-safe manner.
4.  **Bill Pugh Singleton**: Uses an inner static helper class for initialization, which ensures thread-safety and lazy initialization.

#### Example: Eager Initialization

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

#### Example: Lazy Initialization

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

#### Example: Thread-safe Singleton

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

#### Example: Bill Pugh Singleton

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

### Pros

1.  **Controlled Access to the Single Instance**: It provides a controlled access point for the unique instance.
2.  **Reduced Namespace Pollution**: It avoids unnecessary duplication of objects.
3.  **Flexibility**: Singleton patterns can be extended to support a variable number of instances.
4.  **Consistent Data**: Ensures that a single instance holds all the necessary state and data, leading to consistent behavior across the application.

### Cons

1.  **Difficulty in Testing**: Singleton classes can be difficult to unit test because they carry state and often use global access points.
2.  **Hidden Dependencies**: Singleton can introduce hidden dependencies into a system as it provides a global point of access.
3.  **Concurrency Issues**: If not implemented correctly, Singleton can lead to issues in a multithreaded environment.
4.  **Global State**: Singleton can encourage the use of global state, which can make the system harder to understand and maintain.

### Real-Life Example: Database Connection Manager

In many applications, managing database connections is critical. The Database Connection Manager should ensure that only one connection pool exists throughout the application to manage database connections efficiently.

#### DatabaseConnectionManager.java

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

#### Usage Example

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


## Factory Method Pattern

### Introduction

The Factory Method Pattern is a creational design pattern that provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created. This pattern enables a class to defer instantiation to its subclasses, promoting loose coupling and scalability.

### Problem It Solves

The Factory Method Pattern solves the problem of creating objects without specifying the exact class of the object that will be created. It addresses the following issues:

1.  **Decoupling**: Reduces the dependency of a class on concrete classes by relying on interfaces or abstract classes.
2.  **Extensibility**: Makes it easier to introduce new classes with minimal changes to existing code.
3.  **Simplified Object Creation**: Encapsulates the object creation logic in one place, making the code easier to manage and understand.

### How to Implement It
![Factory Method Pattern](https://github.com/user-attachments/assets/a5c7e7af-b6af-4b16-a0b4-f9225920a546)

To implement the Factory Method Pattern, follow these steps:

1.  **Define a Product Interface or Abstract Class**: This defines the type of object that the factory method will create.
2.  **Implement Concrete Products**: These are the actual objects that will be created by the factory method.
3.  **Create a Creator Abstract Class or Interface**: This declares the factory method, which returns an object of type Product.
4.  **Implement Concrete Creators**: These override the factory method to return an instance of a concrete product.

### Detailed Java Example

Let's consider a real-life example where we have a `Notification` system. Different types of notifications (Email, SMS, Push) need to be created, but the client code should not be dependent on the concrete classes.

#### Product Interface

```java
// Notification.java

public interface Notification {
    void notifyUser();
}
```

#### Concrete Products

```java
// EmailNotification.java

public class EmailNotification implements Notification {
    @Override
    public void notifyUser() {
        System.out.println("Sending an email notification");
    }
}
```
```java
// SMSNotification.java

public class SMSNotification implements Notification {
    @Override
    public void notifyUser() {
        System.out.println("Sending an SMS notification");
    }
}
```

```java
// PushNotification.java

public class PushNotification implements Notification {
    @Override
    public void notifyUser() {
        System.out.println("Sending a push notification");
    }
}
```

#### Creator Abstract Class

```java
// NotificationFactory.java

public abstract class NotificationFactory {
    public abstract Notification createNotification();

    public void notifyUser() {
        Notification notification = createNotification();
        notification.notifyUser();
    }
}
```

#### Concrete Creators

```java
// EmailNotificationFactory.java

public class EmailNotificationFactory extends NotificationFactory {
    @Override
    public Notification createNotification() {
        return new EmailNotification();
    }
}
```
``` java
// SMSNotificationFactory.java

public class SMSNotificationFactory extends NotificationFactory {
    @Override
    public Notification createNotification() {
        return new SMSNotification();
    }
}
```
```java
// PushNotificationFactory.java

public class PushNotificationFactory extends NotificationFactory {
    @Override
    public Notification createNotification() {
        return new PushNotification();
    }
}
```

#### Client Code

```java
// Main.java

public class Main {
    public static void main(String[] args) {
        NotificationFactory emailFactory = new EmailNotificationFactory();
        emailFactory.notifyUser();

        NotificationFactory smsFactory = new SMSNotificationFactory();
        smsFactory.notifyUser();

        NotificationFactory pushFactory = new PushNotificationFactory();
        pushFactory.notifyUser();
    }
}
```

### Pros

1.  **Loose Coupling**: The client code is decoupled from the concrete classes, making it easier to manage and extend.
2.  **Single Responsibility Principle**: The creation logic is encapsulated in the factory classes, adhering to the Single Responsibility Principle.
3.  **Open/Closed Principle**: New product types can be introduced without modifying existing code, following the Open/Closed Principle.

### Cons

1.  **Complexity**: Introduces additional classes and interfaces, which can make the code more complex.
2.  **Overhead**: If the number of concrete products is small, the pattern might introduce unnecessary overhead.

The Factory Method Pattern is a powerful design pattern that promotes flexibility and scalability in the creation of objects. By abstracting the instantiation process, it allows for easy extension and modification, making the codebase more maintainable and adaptable to change.

<hr>


## Abstract Factory Pattern

### Introduction

The Abstract Factory Pattern is a creational design pattern that provides an interface for creating families of related or dependent objects without specifying their concrete classes. It is useful when a system needs to be independent of how its objects are created, composed, and represented.

### Problem It Solves

The Abstract Factory Pattern addresses several key issues:

1.  **Family of Products**: It is useful when there are multiple families of products that need to be created together.
2.  **Encapsulation of Object Creation**: It encapsulates the creation logic for a set of related objects, making the system more modular.
3.  **Interchangeability**: It allows the interchange of product families without modifying the client code.

### How to Implement It

![abstract-factory-uml](https://github.com/user-attachments/assets/22827924-0600-4970-bf90-2bf6f4908468)


To implement the Abstract Factory Pattern, follow these steps:

1.  **Define Abstract Product Interfaces**: These interfaces declare the operations that all concrete products must implement.
2.  **Create Concrete Product Classes**: These are specific implementations of the abstract products.
3.  **Define Abstract Factory Interface**: This interface declares methods for creating each type of product.
4.  **Implement Concrete Factory Classes**: These factories create instances of the concrete product classes.

### Detailed Java Example

Let's consider a real-life example where we have a GUI toolkit that should work with multiple operating systems (Windows and Mac). The GUI toolkit needs to create different types of buttons and checkboxes depending on the operating system.

#### Abstract Product Interfaces

```java
// Button.java

public interface Button {
    void paint();
}
```

```java
// Checkbox.java

public interface Checkbox {
    void paint();
}
```

#### Concrete Product Classes

``` java
// WindowsButton.java

public class WindowsButton implements Button {
    @Override
    public void paint() {
        System.out.println("Rendering a button in Windows style");
    }
}
```

```java
// MacButton.java

public class MacButton implements Button {
    @Override
    public void paint() {
        System.out.println("Rendering a button in Mac style");
    }
}
```

```java
// WindowsCheckbox.java

public class WindowsCheckbox implements Checkbox {
    @Override
    public void paint() {
        System.out.println("Rendering a checkbox in Windows style");
    }
}
```

```java
// MacCheckbox.java

public class MacCheckbox implements Checkbox {
    @Override
    public void paint() {
        System.out.println("Rendering a checkbox in Mac style");
    }
}
```

#### Abstract Factory Interface

```java
// GUIFactory.java

public interface GUIFactory {
    Button createButton();
    Checkbox createCheckbox();
}
```

#### Concrete Factory Classes

```java
// WindowsFactory.java

public class WindowsFactory implements GUIFactory {
    @Override
    public Button createButton() {
        return new WindowsButton();
    }

    @Override
    public Checkbox createCheckbox() {
        return new WindowsCheckbox();
    }
}
```

```java
// MacFactory.java

public class MacFactory implements GUIFactory {
    @Override
    public Button createButton() {
        return new MacButton();
    }

    @Override
    public Checkbox createCheckbox() {
        return new MacCheckbox();
    }
}
```

#### Client Code

```java
// Application.java

public class Application {
    private Button button;
    private Checkbox checkbox;

    public Application(GUIFactory factory) {
        button = factory.createButton();
        checkbox = factory.createCheckbox();
    }

    public void paint() {
        button.paint();
        checkbox.paint();
    }
}
```

```java
// Main.java

public class Main {
    public static void main(String[] args) {
        GUIFactory factory;
        String osName = System.getProperty("os.name").toLowerCase();
        if (osName.contains("win")) {
            factory = new WindowsFactory();
        } else {
            factory = new MacFactory();
        }
        Application app = new Application(factory);
        app.paint();
    }
}
```

### Pros

1.  **Encapsulation**: Encapsulates the creation of related objects, promoting modularity and separation of concerns.
2.  **Interchangeability**: Allows easy switching between different families of products.
3.  **Consistency**: Ensures that products created by one factory are compatible with each other.
4.  **Single Responsibility Principle**: Separates the creation of objects from their usage, adhering to the Single Responsibility Principle.

### Cons

1.  **Complexity**: Increases the complexity of the system by introducing additional interfaces and classes.
2.  **Maintenance Overhead**: Adding new product families requires changes to the abstract factory interface and all concrete factories.

The Abstract Factory Pattern is a powerful design pattern that promotes flexibility and scalability in the creation of related objects. By abstracting the instantiation process, it allows for easy extension and modification, making the codebase more maintainable and adaptable to change.

<hr>

## Builder Pattern

### Introduction

The Builder Pattern is a creational design pattern that separates the construction of a complex object from its representation, allowing the same construction process to create different representations. It is particularly useful when an object needs to be constructed in multiple steps or configurations.

### Problem It Solves

The Builder Pattern addresses several key issues:

1.  **Complex Object Construction**: When an object requires numerous steps to construct, the Builder Pattern simplifies the creation process by breaking it down into discrete steps.
2.  **Readability**: Improves the readability of the code by clearly defining the steps required to create an object.
3.  **Immutability**: Often used to create immutable objects with multiple configuration options.
4.  **Separation of Concerns**: Decouples the process of object construction from the final representation, adhering to the Single Responsibility Principle.

### How to Implement It

![builder-uml](https://github.com/user-attachments/assets/6d9a668c-1c30-4fd7-b721-5452a10fc695)

To implement the Builder Pattern, follow these steps:

1.  **Define a Product Class**: This class represents the complex object to be built.
2.  **Create a Builder Interface or Abstract Class**: This declares the methods for creating the different parts of the product.
3.  **Implement Concrete Builder Classes**: These classes build and assemble parts of the product by implementing the builder interface or abstract class.
4.  **Director Class (Optional)**: This class constructs an object using the builder interface. It is optional but can be useful for managing the construction process.
5.  **Client Code**: The client code creates a builder object, passes it to the director, and then retrieves the final product.

### Detailed Java Example

Let's consider a real-life example where we need to construct a complex `Car` object with various attributes like engine, seats, GPS, and trip computer.

#### Product Class

```java
// Car.java

public class Car {
    private String engine;
    private int seats;
    private boolean hasGPS;
    private boolean hasTripComputer;

    // Getters and setters
    public void setEngine(String engine) {
        this.engine = engine;
    }

    public void setSeats(int seats) {
        this.seats = seats;
    }

    public void setHasGPS(boolean hasGPS) {
        this.hasGPS = hasGPS;
    }

    public void setHasTripComputer(boolean hasTripComputer) {
        this.hasTripComputer = hasTripComputer;
    }

    @Override
    public String toString() {
        return "Car [engine=" + engine + ", seats=" + seats + ", hasGPS=" + hasGPS + ", hasTripComputer=" + hasTripComputer + "]";
    }
}
```

#### Builder Interface

```java
// CarBuilder.java

public interface CarBuilder {
    void reset();
    void setEngine(String engine);
    void setSeats(int seats);
    void setGPS(boolean hasGPS);
    void setTripComputer(boolean hasTripComputer);
    Car getResult();
}
```

#### Concrete Builder Class

``` java
// SportsCarBuilder.java

public class SportsCarBuilder implements CarBuilder {
    private Car car;

    public SportsCarBuilder() {
        this.car = new Car();
    }

    @Override
    public void reset() {
        this.car = new Car();
    }

    @Override
    public void setEngine(String engine) {
        car.setEngine(engine);
    }

    @Override
    public void setSeats(int seats) {
        car.setSeats(seats);
    }

    @Override
    public void setGPS(boolean hasGPS) {
        car.setHasGPS(hasGPS);
    }

    @Override
    public void setTripComputer(boolean hasTripComputer) {
        car.setHasTripComputer(hasTripComputer);
    }

    @Override
    public Car getResult() {
        return this.car;
    }
}
```

```java 
// CityCarBuilder.java

public class CityCarBuilder implements CarBuilder {
    private Car car;

    public CityCarBuilder() {
        this.car = new Car();
    }

    @Override
    public void reset() {
        this.car = new Car();
    }

    @Override
    public void setEngine(String engine) {
        car.setEngine(engine);
    }

    @Override
    public void setSeats(int seats) {
        car.setSeats(seats);
    }

    @Override
    public void setGPS(boolean hasGPS) {
        car.setHasGPS(hasGPS);
    }

    @Override
    public void setTripComputer(boolean hasTripComputer) {
        car.setHasTripComputer(hasTripComputer);
    }

    @Override
    public Car getResult() {
        return this.car;
    }
}
```

#### Director Class (Optional)

```java
// CarDirector.java

public class CarDirector {
    public void constructSportsCar(CarBuilder builder) {
        builder.reset();
        builder.setEngine("V8");
        builder.setSeats(2);
        builder.setGPS(true);
        builder.setTripComputer(true);
    }

    public void constructCityCar(CarBuilder builder) {
        builder.reset();
        builder.setEngine("V4");
        builder.setSeats(4);
        builder.setGPS(true);
        builder.setTripComputer(false);
    }
}
```

#### Client Code

```java
// Main.java

public class Main {
    public static void main(String[] args) {
        CarDirector director = new CarDirector();

        CarBuilder sportsCarBuilder = new SportsCarBuilder();
        director.constructSportsCar(sportsCarBuilder);
        Car sportsCar = sportsCarBuilder.getResult();
        System.out.println("Sports Car: " + sportsCar);

        CarBuilder cityCarBuilder = new CityCarBuilder();
        director.constructCityCar(cityCarBuilder);
        Car cityCar = cityCarBuilder.getResult();
        System.out.println("City Car: " + cityCar);
    }
}
```

### Pros

1.  **Flexibility**: The same construction process can create different representations of the product.
2.  **Readability**: The code for constructing an object is more readable and maintainable.
3.  **Control**: Provides fine-grained control over the construction process.
4.  **Immutability**: Facilitates the creation of immutable objects.

### Cons

1.  **Complexity**: Increases the complexity of the code with additional builder and director classes.
2.  **Overhead**: May add unnecessary overhead if the construction process is simple and doesn't benefit from the Builder Pattern.

The Builder Pattern is a powerful design pattern for constructing complex objects. By decoupling the construction process from the final representation, it provides flexibility, readability, and control, making it easier to manage and extend complex object creation.

<hr>

## Prototype Pattern

### Introduction

The Prototype Pattern is a creational design pattern used to create objects by copying an existing object, known as the prototype. This pattern is particularly useful when the cost of creating a new instance of a class is more expensive than copying an existing instance. The Prototype Pattern allows for the creation of new objects by cloning an existing object, enabling efficient and flexible object creation.

### What Problem It Solves

The Prototype Pattern solves several problems, including:

1.  **Costly Object Creation**: When the cost of creating a new object is high (e.g., when it involves resource-intensive operations such as database access or network communication), cloning an existing object can be more efficient.
2.  **Complex Object Construction**: When an object's creation process involves a complex series of steps, copying an existing object can simplify and expedite the process.
3.  **Avoiding Subclass Explosion**: When there are many subclasses of a class, each with a different configuration, the Prototype Pattern can reduce the need for numerous subclasses by enabling object creation through cloning.

### How to Implement It
![prototype-pattern](https://github.com/user-attachments/assets/fe16b1b3-ccf7-4f0d-b104-9b8c98ea6a51)


To implement the Prototype Pattern, follow these steps:

1.  **Create a Prototype Interface**: Define an interface with a method for cloning objects.
2.  **Implement the Prototype Interface**: Implement the interface in the classes that need to be cloned.
3.  **Clone Objects**: Use the clone method to create new objects by copying existing ones.

Here is an example in Java:

``` java
// Prototype Interface

public interface Prototype {
    Prototype clone();
}
```

``` java
// Concrete Prototype Class

public class Car implements Prototype {
    private String model;
    private String color;
    private int year;

    public Car(String model, String color, int year) {
        this.model = model;
        this.color = color;
        this.year = year;
    }

    public String getModel() {
        return model;
    }

    public String getColor() {
        return color;
    }

    public int getYear() {
        return year;
    }

    @Override
    public Car clone() {
        return new Car(this.model, this.color, this.year);
    }

    @Override
    public String toString() {
        return "Car{" +
                "model='" + model + '\'' +
                ", color='" + color + '\'' +
                ", year=" + year +
                '}';
    }
}
```

``` java
// Client Code

public class Main {
    public static void main(String[] args) {
        Car originalCar = new Car("Tesla Model S", "Red", 2022);
        Car clonedCar = originalCar.clone();

        System.out.println("Original Car: " + originalCar);
        System.out.println("Cloned Car: " + clonedCar);
    }
}
```

In this example, the `Car` class implements the `Prototype` interface, allowing objects of the `Car` class to be cloned. The `clone` method creates a new `Car` object with the same properties as the original.

#### Pros
1.  **Efficient Object Creation**: Cloning an existing object is often faster and less resource-intensive than creating a new object from scratch.
2.  **Simplified Object Construction**: Cloning simplifies the creation of complex objects by copying an existing instance.
3.  **Reduced Subclass Explosion**: The Prototype Pattern reduces the need for numerous subclasses by allowing objects to be created through cloning.

### Cons

1.  **Deep vs. Shallow Copying**: Implementing cloning can be complex, especially when dealing with deep copying (copying objects that contain references to other objects).
2.  **Cloning Complex Objects**: If an object contains complex internal structures or circular references, implementing cloning can be challenging.
3.  **Copying State**: Ensuring that the copied object's state is correct and independent of the original object can be difficult.

### Real-Life Java Example

Consider a scenario where you need to create a large number of documents with similar content but slight variations. The Prototype Pattern can be used to clone a template document and make the necessary modifications.

```java
// Prototype Interface

public interface DocumentPrototype {
    DocumentPrototype clone();
}
```

``` java
// Concrete Prototype Class

public class Document implements DocumentPrototype {
    private String title;
    private String content;

    public Document(String title, String content) {
        this.title = title;
        this.content = content;
    }

    public String getTitle() {
        return title;
    }

    public String getContent() {
        return content;
    }

    public void setTitle(String title) {
        this.title = title;
    }

    public void setContent(String content) {
        this.content = content;
    }

    @Override
    public Document clone() {
        return new Document(this.title, this.content);
    }

    @Override
    public String toString() {
        return "Document{" +
                "title='" + title + '\'' +
                ", content='" + content + '\'' +
                '}';
    }
}
```

```java
// Client Code

public class Main {
    public static void main(String[] args) {
        Document template = new Document("Template Title", "Template Content");
        Document report = template.clone();
        report.setTitle("Monthly Report");
        report.setContent("This is the content of the monthly report.");

        Document invoice = template.clone();
        invoice.setTitle("Invoice");
        invoice.setContent("This is the content of the invoice.");

        System.out.println("Template Document: " + template);
        System.out.println("Report Document: " + report);
        System.out.println("Invoice Document: " + invoice);
    }
}
```

In this example, the `Document` class implements the `DocumentPrototype` interface, allowing objects of the `Document` class to be cloned. The client code demonstrates how a template document can be cloned and modified to create different types of documents (e.g., reports, invoices) efficiently.

<hr>

## Structural Patterns

Structural patterns focus on how classes and objects can be composed to form larger, more complex structures. They facilitate design by identifying simple ways to realize relationships between entities. These patterns help ensure that the parts of a system work together in a flexible and efficient manner, making the system more robust and easier to manage.

### Purpose of Structural Patterns

1.  **Composition of Objects and Classes**: They deal with the composition of objects and classes to create larger structures, promoting reuse and flexibility.
2.  **Simplification of Interfaces**: Structural patterns often provide simplified interfaces to complex subsystems, making them easier to use.
3.  **Promotion of Loose Coupling**: By defining clear interfaces and abstracting relationships, these patterns reduce the dependency between system components, promoting loose coupling.

### Common Characteristics

1.  **Class and Object Composition**: These patterns are concerned with how classes and objects are composed to form larger structures.
2.  **Interface Simplification**: They often provide simplified interfaces to complex subsystems or objects, enhancing usability.
3.  **Decoupling**: Structural patterns promote decoupling of components by abstracting relationships and interactions.

### Benefits

1.  **Improved Flexibility**: By defining clear and flexible compositions, structural patterns allow for easy modification and extension of the system.
2.  **Enhanced Reusability**: These patterns promote the reuse of existing components by composing them in various ways.
3.  **Simplified Maintenance**: Simplified interfaces and decoupled components make the system easier to maintain and extend.

### When to Use

1.  **When Dealing with Complex Structures**: Structural patterns are beneficial when you need to manage and simplify complex structures of objects and classes.
2.  **When Simplifying Interfaces**: Use these patterns to provide simplified interfaces to complex subsystems, making them easier to use and understand.
3.  **When Promoting Reusability and Flexibility**: They are useful when you need to promote reuse and flexibility by composing existing components in various ways.

Understanding and applying structural patterns is essential for building flexible, maintainable, and scalable systems. This repository aims to provide a comprehensive guide to various structural patterns in Java, helping you incorporate these best practices into your projects.

<hr>

## [Adapter Pattern](#adapter-pattern)

### Introduction

The Adapter Pattern is a structural design pattern that allows objects with incompatible interfaces to work together. It acts as a bridge between two incompatible interfaces, converting the interface of a class into another interface that a client expects. This pattern is particularly useful when integrating legacy code with new code, or when you want to use a class that does not match the interface you need.

#### What Problem It Solves

The Adapter Pattern addresses the issue of incompatible interfaces by providing a way to make existing classes work with others without modifying their source code. It allows for flexibility and reusability by enabling objects with different interfaces to collaborate seamlessly.

#### How to Implement It
![adaptor-pattern](https://github.com/user-attachments/assets/7e7e9a1e-51ca-4ce2-9be2-a21750ad92ab)

1.  **Identify Incompatible Interfaces**: Determine the interfaces that need to work together but are incompatible.
2.  **Create an Adapter Class**: Implement an adapter class that implements the expected interface and translates the calls from the client to the adaptee.
3.  **Use the Adapter**: Replace direct calls to the adaptee with calls to the adapter.

#### Pros

1.  **Increased Flexibility**: The Adapter Pattern allows you to use existing classes without modifying them, increasing the flexibility of your code.
2.  **Promotes Reusability**: By allowing incompatible interfaces to work together, the adapter pattern promotes the reuse of existing components.
3.  **Decoupling**: It decouples the client code from the adaptee, making the system more maintainable and easier to extend.

#### Cons

1.  **Complexity**: Introducing an adapter adds an extra layer of complexity to the code, which might be unnecessary for simple scenarios.
2.  **Overhead**: The adapter can introduce a performance overhead, as it translates calls between interfaces.

#### Real-Life Java Example

Consider a scenario where you have an existing `AudioPlayer` class that plays audio files and you want to integrate a new `MediaPlayer` interface that supports both audio and video playback. The `AudioPlayer` class is not compatible with the `MediaPlayer` interface. You can use the Adapter Pattern to make them work together.

```java
// Target Interface -

// MediaPlayer.java
interface MediaPlayer {
    void play(String audioType, String fileName);
}
```
```java
// Adaptee Class -

// AudioPlayer.java
class AudioPlayer {
    public void playAudio(String fileName) {
        System.out.println("Playing audio file. Name: " + fileName);
    }
}
```
```java
// Adapter Class -

// MediaAdapter.java
class MediaAdapter implements MediaPlayer {
    private AudioPlayer audioPlayer;

    public MediaAdapter(AudioPlayer audioPlayer) {
        this.audioPlayer = audioPlayer;
    }

    @Override
    public void play(String audioType, String fileName) {
        if (audioType.equalsIgnoreCase("audio")) {
            audioPlayer.playAudio(fileName);
        } else {
            System.out.println("Invalid media. " + audioType + " format not supported");
        }
    }
}
```
```java
// Client Class -

// AudioPlayerClient.java
class AudioPlayerClient {
    private MediaPlayer mediaPlayer;

    public AudioPlayerClient(MediaPlayer mediaPlayer) {
        this.mediaPlayer = mediaPlayer;
    }

    public void play(String audioType, String fileName) {
        mediaPlayer.play(audioType, fileName);
    }

    public static void main(String[] args) {
        AudioPlayer audioPlayer = new AudioPlayer();
        MediaAdapter mediaAdapter = new MediaAdapter(audioPlayer);
        AudioPlayerClient client = new AudioPlayerClient(mediaAdapter);

        client.play("audio", "song.mp3");
        client.play("video", "movie.mp4");
    }
}
```

In this example:

1.  **MediaPlayer Interface**: Defines the target interface that the client expects.
2.  **AudioPlayer Class**: Represents the existing class that needs to be adapted.
3.  **MediaAdapter Class**: Implements the `MediaPlayer` interface and translates calls to the `AudioPlayer` class.
4.  **AudioPlayerClient Class**: Demonstrates how to use the adapter to play different types of media.

The `MediaAdapter` class makes it possible for the `AudioPlayer` class to be used where a `MediaPlayer` is expected, solving the problem of incompatible interfaces.

Understanding and applying the Adapter Pattern is crucial for integrating different parts of a system and making them work together seamlessly. This pattern enhances the flexibility and reusability of your code, making it a valuable tool in software design.

<hr>

## [Bridge Pattern](#bridge-pattern)

### Introduction

The Bridge Pattern is a structural design pattern that separates an object's abstraction from its implementation, allowing the two to vary independently. It is used to decouple abstraction and implementation so that they can be developed and modified separately. This pattern is particularly useful when both the abstraction and the implementation may evolve over time and need to be changed independently.

### What Problem It Solves

The Bridge Pattern addresses the issue of tight coupling between an abstraction and its implementation. In scenarios where multiple abstractions and implementations need to be combined, the bridge pattern helps in managing the complexity by keeping the abstraction and implementation separate. This leads to a more flexible and maintainable codebase.

### How to Implement It

![bridge-pattern](https://github.com/user-attachments/assets/710abd39-f1cc-423c-a837-0daf5726ca42)

1.  **Define the Abstraction**: Create an abstract class that contains a reference to an implementation object.
2.  **Create Implementor Interface**: Define an interface for the implementation part, which the abstraction will use.
3.  **Concrete Implementations**: Implement the concrete classes that follow the Implementor interface.
4.  **Refine Abstraction**: Extend the abstraction class to include any additional features or functionality.

### Pros

1.  **Decoupling**: The Bridge Pattern decouples the abstraction from the implementation, allowing them to vary independently.
2.  **Increased Flexibility**: It enables the abstraction and implementation to be extended and changed independently, promoting flexibility.
3.  **Improved Maintainability**: Changes in one part of the code (abstraction or implementation) do not affect the other part, making the code easier to maintain.

### Cons

1.  **Complexity**: The pattern can increase the complexity of the code due to the creation of multiple abstraction and implementation classes.
2.  **Initial Effort**: It may require significant initial effort to set up the bridge structure, especially in systems that are already tightly coupled.

### Real-Life Java Example

Consider a scenario where you have different types of remote controls (e.g., basic remote, advanced remote) and different types of devices (e.g., TV, radio). Using the Bridge Pattern, you can decouple the remote controls from the devices.

```java
// Implementor Interface

// Device.java
interface Device {
    void turnOn();
    void turnOff();
    void setVolume(int volume);
}
```

```java
// Concrete Implementor 1

// TV.java
class TV implements Device {
    private int volume;

    @Override
    public void turnOn() {
        System.out.println("Turning on the TV");
    }

    @Override
    public void turnOff() {
        System.out.println("Turning off the TV");
    }

    @Override
    public void setVolume(int volume) {
        this.volume = volume;
        System.out.println("Setting TV volume to " + volume);
    }
}
```

```java
// Concrete Implementor 2

// Radio.java
class Radio implements Device {
    private int volume;

    @Override
    public void turnOn() {
        System.out.println("Turning on the Radio");
    }

    @Override
    public void turnOff() {
        System.out.println("Turning off the Radio");
    }

    @Override
    public void setVolume(int volume) {
        this.volume = volume;
        System.out.println("Setting Radio volume to " + volume);
    }
}
```

```java
// Abstraction

// RemoteControl.java
abstract class RemoteControl {
    protected Device device;

    protected RemoteControl(Device device) {
        this.device = device;
    }

    abstract void turnOn();
    abstract void turnOff();
    abstract void setVolume(int volume);
}
```

```java
// Refined Abstraction 1

// BasicRemoteControl.java
class BasicRemoteControl extends RemoteControl {

    protected BasicRemoteControl(Device device) {
        super(device);
    }

    @Override
    public void turnOn() {
        device.turnOn();
    }

    @Override
    public void turnOff() {
        device.turnOff();
    }

    @Override
    public void setVolume(int volume) {
        device.setVolume(volume);
    }
}
```

```java
// Refined Abstraction 2

// AdvancedRemoteControl.java
class AdvancedRemoteControl extends RemoteControl {

    protected AdvancedRemoteControl(Device device) {
        super(device);
    }

    @Override
    public void turnOn() {
        device.turnOn();
    }

    @Override
    public void turnOff() {
        device.turnOff();
    }

    @Override
    public void setVolume(int volume) {
        device.setVolume(volume);
    }

    public void mute() {
        device.setVolume(0);
        System.out.println("Muting the device");
    }
}
```

```java
// Client Code

// BridgePatternDemo.java
public class BridgePatternDemo {
    public static void main(String[] args) {
        Device tv = new TV();
        RemoteControl basicRemote = new BasicRemoteControl(tv);
        RemoteControl advancedRemote = new AdvancedRemoteControl(tv);

        basicRemote.turnOn();
        basicRemote.setVolume(10);
        basicRemote.turnOff();

        advancedRemote.turnOn();
        advancedRemote.setVolume(20);
        advancedRemote.mute();
        advancedRemote.turnOff();
    }
}
```

In this example:

1.  **Device Interface**: Represents the implementor interface that defines the basic operations for devices.
2.  **TV and Radio Classes**: Concrete implementations of the `Device` interface.
3.  **RemoteControl Abstract Class**: Acts as the abstraction that contains a reference to a `Device` object.
4.  **BasicRemoteControl and AdvancedRemoteControl Classes**: Refined abstractions that extend the `RemoteControl` class.
5.  **BridgePatternDemo Class**: Demonstrates how to use the bridge pattern to control different devices using different remote controls.

The Bridge Pattern helps in decoupling the remote controls from the devices, allowing them to vary independently. This makes the system more flexible, maintainable, and scalable.

<br>

<hr>

## [Decorator Pattern](#decorator-pattern)

### Introduction

The Decorator Pattern is a structural design pattern that allows behavior to be added to individual objects, either statically or dynamically, without affecting the behavior of other objects from the same class. It is typically used to extend the functionalities of classes in a flexible and reusable manner.

### What Problem It Solves

The Decorator Pattern addresses the need for extending the behavior of objects without altering their structure. It provides an alternative to subclassing for extending functionality. This pattern is particularly useful when you want to add responsibilities to objects dynamically and transparently, without affecting other instances of the same class.

### How to Implement It
![decorator-pattern](https://github.com/user-attachments/assets/535eac2d-0d82-4b77-a33c-2d5abeca998d)

1.  **Component Interface**: Define an interface that both the concrete component and the decorators will implement.
2.  **Concrete Component**: Create a class that implements the component interface.
3.  **Decorator Class**: Create an abstract decorator class that implements the component interface and contains a reference to a component object.
4.  **Concrete Decorators**: Implement concrete decorator classes that extend the decorator class and add new behaviors.

### Pros

1.  **Flexibility**: Allows adding functionalities to objects at runtime, enhancing flexibility.
2.  **Reusability**: Promotes code reuse by allowing the combination of various decorators to create new behaviors.
3.  **Single Responsibility Principle**: Each decorator class can focus on a single concern, adhering to the single responsibility principle.

### Cons

1.  **Complexity**: The pattern can introduce complexity due to the creation of many small classes.
2.  **Maintenance**: Managing and maintaining a large number of decorator classes can be challenging.

### Real-Life Java Example

Consider a scenario where you have a simple `Coffee` interface and you want to add different flavors and ingredients to the coffee dynamically.

```java
// Component Interface

// Coffee.java
interface Coffee {
    String getDescription();
    double getCost();
}
```

```java
// Concrete Component

// SimpleCoffee.java
class SimpleCoffee implements Coffee {

    @Override
    public String getDescription() {
        return "Simple coffee";
    }

    @Override
    public double getCost() {
        return 5.0;
    }
}
```

```java
// Decorator Class

// CoffeeDecorator.java
abstract class CoffeeDecorator implements Coffee {
    protected Coffee decoratedCoffee;

    public CoffeeDecorator(Coffee coffee) {
        this.decoratedCoffee = coffee;
    }

    @Override
    public String getDescription() {
        return decoratedCoffee.getDescription();
    }

    @Override
    public double getCost() {
        return decoratedCoffee.getCost();
    }
}
```

```java
// Concrete Decorator

// MilkDecorator.java
class MilkDecorator extends CoffeeDecorator {

    public MilkDecorator(Coffee coffee) {
        super(coffee);
    }

    @Override
    public String getDescription() {
        return decoratedCoffee.getDescription() + ", milk";
    }

    @Override
    public double getCost() {
        return decoratedCoffee.getCost() + 1.5;
    }
}
```

```java
// Concrete Decorator

// SugarDecorator.java
class SugarDecorator extends CoffeeDecorator {

    public SugarDecorator(Coffee coffee) {
        super(coffee);
    }

    @Override
    public String getDescription() {
        return decoratedCoffee.getDescription() + ", sugar";
    }

    @Override
    public double getCost() {
        return decoratedCoffee.getCost() + 0.5;
    }
}
```

```java
// Concrete Decorators

// VanillaDecorator.java
class VanillaDecorator extends CoffeeDecorator {

    public VanillaDecorator(Coffee coffee) {
        super(coffee);
    }

    @Override
    public String getDescription() {
        return decoratedCoffee.getDescription() + ", vanilla";
    }

    @Override
    public double getCost() {
        return decoratedCoffee.getCost() + 2.0;
    }
}
```

```java
// Client Code

// DecoratorPatternDemo.java
public class DecoratorPatternDemo {
    public static void main(String[] args) {
        Coffee coffee = new SimpleCoffee();
        System.out.println(coffee.getDescription() + " $" + coffee.getCost());

        coffee = new MilkDecorator(coffee);
        System.out.println(coffee.getDescription() + " $" + coffee.getCost());

        coffee = new SugarDecorator(coffee);
        System.out.println(coffee.getDescription() + " $" + coffee.getCost());

        coffee = new VanillaDecorator(coffee);
        System.out.println(coffee.getDescription() + " $" + coffee.getCost());
    }
}
```

In this example:

1.  **Coffee Interface**: Defines the common interface for both the concrete component and decorators.
2.  **SimpleCoffee Class**: A concrete component that implements the `Coffee` interface.
3.  **CoffeeDecorator Class**: An abstract class that implements the `Coffee` interface and holds a reference to a `Coffee` object.
4.  **MilkDecorator, SugarDecorator, VanillaDecorator Classes**: Concrete decorators that extend the `CoffeeDecorator` class and add their specific behavior.
5.  **DecoratorPatternDemo Class**: Demonstrates the use of the Decorator Pattern by dynamically adding behaviors (milk, sugar, vanilla) to a simple coffee object.

The Decorator Pattern allows you to enhance the functionality of an object dynamically and transparently, making the system more flexible and easier to extend.

<br>

<hr>



## Contributing

### How to Contribute

Fork the repository, make your changes, and submit a pull request. 


### License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/AkshayChandole/Java_System_Design_Patterns/blob/main/LICENSE) file for details.
