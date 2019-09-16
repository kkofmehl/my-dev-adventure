# Demystifying Dependency Injection

What is dependency injection?

>Dependency Injection -> Wikipedia, 2016

## SOLID Principles

### Single Responsibility Principle
- Classes and objects should have a single purpose  (avoid the "Utility" class)

### Open/Closed Principle
- People can inherit from a class but don't change base implementation

### Liskov Substitution Principle
- Any sub-class should be able to replace its parent class

### Interface Segregation Principle
- Interfaces should be numerous and small.
- Interface should be minimalistic in nature (2-3 methods to implement)

### Dependency Inversion Principle
- High level modules should not depend on lower-level modules, they should depend on abstractions.
- "I should not be in charge of the things I'm dependent upon"

## Why do we want loosely coupled code? Really.

I want my code to not be like spaghetti and more like lego bricks

Benefits:
- Code maintenance is easy
- Easier to write tests against
- Flexible Configuration
- Teams can work in parallel

## Consequences of using Dependency Injection
- More difficult to trace (adding more abstraction)
- Takes extra effort on the front-end
- Explosion of types
- Can create a dependency on a DI framework

## Types of Dependency Injection (in order of popularity)

- Constructor Injection (most common)
    - Dependencies are passed into a class via the contructor
- Property Injection
    - If you are using this method, you should always provide a default value
- Method Injection
    - If a class has a method that has a dependency, we pass the dependency as a parameter to just the method
- Service Locator
    - You have a static class that serves up a dependency upon request. (been used for a long time)
- Others

Demo App Layout
- Application Layers
    - Composition Root
    - View
    - Presentation
    - Business Logic
    - Repositories
    - Data Access
- Other
    - Shared Components

> If you are wanting to implement DI, be aware of "new" keyword within constructors.  These can hint at "code smell"

