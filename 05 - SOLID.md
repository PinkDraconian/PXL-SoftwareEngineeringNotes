---
title: 05 - SOLID
created: '2020-11-25T20:02:44.772Z'
modified: '2020-11-25T20:10:40.647Z'
---

# 05 - SOLID
## SOLID
- Single Responsibility
- Open closed
- Liskov Substution
- Interface Segregation
- Dependency Inversion

## SOLID - Single Responsibility
Every object should ahve a single responsibility and all of it services should be alligned with that.
Responsibility = Reason to change

## SOLID - Open Closed
- Open for extension
- Closed for modification
Building on top of classes by subclassing and polymorphism, rather than modifying their code

## SOLID - Liskov Substitution
Subclasses should be substitutable for the classes from which they were derived (Duck with batteries is not a duck)

## SOLID - Interface Segregation
Clients should not be forced to depend on methods they don't use. If a class exposes so members that those members can be broken down into groups that serve different clients that don't use members from other groups, then expose them as interfaces

## SOLID - Dependency Inversion 
High level modules shouldn't depend on low-level modules but should both depend on shared abstractions. (Stopcontact)
