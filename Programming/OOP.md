# The four principles of OOP

## Encapsulation

* Refer to building data inside methods that can operate on that data within a class.
* Hiding data inside a class, preventing components outside the class from directly interacting with it.
* Outside components can only interact with attributes of the class through the class's methods.
* Getters and Setters can be used to
This helps with maintenance and decreasing code complexity.

## Abstraction

* Showing only essential details and hiding everything else.
* 

## Inheritence

## Polymorphism

# SOLID Principles

## Single Responsibility

A class should only be responsible for one thing.

## Open/Close

Software entities should be open for extension, but closed for modification.

(i.e. you shouldn't have to modify a class afer creating it, rather interfaces and/or abstract classes should be used as to allow new sub classes to implement their own specifications)

## Liskov Substitution

Only use inheritence when a subclass can be used as a replacement for the superclass.

## Interface Segregation

Keep interfaces as small as possible.

Classes should not be forced to implement interfaces they don't use.

## Dependency Inversion

Depend on interfaces and / or abstractions and not concrete classes.