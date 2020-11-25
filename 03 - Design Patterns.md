---
title: 03 - Design Patterns
created: '2020-10-07T18:23:15.479Z'
modified: '2020-10-22T19:40:26.320Z'
---

# 03 - Design Patterns 
## Design principles
- Identify the aspects of your application that vary and separate them from what stays the same
- Program to an interface, not an implementation
- Favor composition over inheritance
- Strive for loosely coupled designs between objects that interact

## Strategy
Defines a famility of algorithms, encapsulates each one, and makes them interchangeable
Strategy lets the algorithm vary independently from clients that use it

## Observer
Defines a one-to-many dependency between objects so that when one object changes state, all of its dependents are notified and updated automatically
- Loose coupling

## State
Allows an object to alter its behavior when its internal state changes. The object will appear to change its class.

### Difference between state and strategy
- Strategy: Not often changed in runtime
- State: Delegate behaviour often changed at runtime
