# System Design: Low-Level Design (LLD)

Notes and practice for learning LLD for interviews.

## Roadmap

### 1. Foundations
- [ ] OOP: encapsulation, abstraction, inheritance, polymorphism
- [ ] Class relationships: association, aggregation, composition, dependency
- [ ] UML class and sequence diagrams

### 2. Design principles
- [ ] SOLID
- [ ] DRY, KISS, YAGNI
- [ ] Composition over inheritance

### 3. Design patterns
- [ ] Creational: Singleton, Factory Method, Abstract Factory, Builder
- [ ] Structural: Adapter, Decorator, Facade, Proxy, Composite
- [ ] Behavioral: Strategy, Observer, State, Command, Chain of Responsibility

### 4. Concurrency
- [ ] Threads, locks and synchronization
- [ ] Producer-consumer
- [ ] Thread-safe class design

## Practice problems: top 20 LLD interview questions

A curated set of commonly asked problems. Difficulty is a suggested study order, not an official ranking.

| TopicName | Difficulty | Link |
|---|---|---|
| Tic-Tac-Toe | Basic | |
| Snake and Ladder | Basic | |
| Vending Machine | Basic | |
| Logging Framework | Basic | |
| LRU Cache | Basic | |
| Parking Lot | Easy | |
| ATM | Easy | |
| Library Management System | Easy | |
| Notification System | Easy | |
| Hotel Management System | Easy | |
| Elevator System | Medium | |
| Splitwise | Medium | |
| Rate Limiter | Medium | |
| Pub-Sub System | Medium | |
| Meeting Scheduler | Medium | |
| Movie Ticket Booking (BookMyShow) | Hard | |
| Chess | Hard | |
| Ride-Sharing Service (Uber) | Hard | |
| Food Delivery Service (Swiggy) | Hard | |
| Online Shopping System (Amazon) | Hard | |

## Interview format

Follow these steps for every question. Times are for a 45-minute round, so scale them to the level.

| Step | What to do | Time |
|---|---|---|
| 1. Requirements | Clarify features, constraints and what is out of scope | 5 min |
| 2. Entities | Identify the core classes and enums | 5 min |
| 3. Class diagram | Define relationships and responsibilities (Mermaid) | 10 min |
| 4. Code | Write key interfaces and the main flow (Java) | 18 min |
| 5. Follow-ups | Edge cases, concurrency and extensibility | 7 min |

Apply design patterns only where they solve a real need.
