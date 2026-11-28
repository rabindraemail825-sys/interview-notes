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

## Practice problems: 21 common LLD interview questions

A curated set of commonly asked problems. Difficulty is a suggested study order, not an official ranking.

| S.No | TopicName | Difficulty | Link |
|---|---|---|---|
| 1 | Tic-Tac-Toe | Basic | [Solution](practice-problems/01-tic-tac-toe.md) |
| 2 | Snake and Ladder | Basic | [Solution](practice-problems/02-snake-and-ladder.md) |
| 3 | Vending Machine | Basic | [Solution](practice-problems/03-vending-machine.md) |
| 4 | Logging Framework | Basic | [Solution](practice-problems/04-logging-framework.md) |
| 5 | LRU Cache | Basic | [Solution](practice-problems/05-lru-cache.md) |
| 6 | Parking Lot | Easy | [Solution](practice-problems/06-parking-lot.md) |
| 7 | ATM | Easy | [Solution](practice-problems/07-atm.md) |
| 8 | Library Management System | Easy | [Solution](practice-problems/08-library-management.md) |
| 9 | Notification System | Easy | [Solution](practice-problems/09-notification-system.md) |
| 10 | Hotel Management System | Easy | [Solution](practice-problems/10-hotel-management.md) |
| 11 | Elevator System | Medium | [Solution](practice-problems/11-elevator-system.md) |
| 12 | Splitwise | Medium | [Solution](practice-problems/12-splitwise.md) |
| 13 | Rate Limiter | Medium | [Solution](practice-problems/13-rate-limiter.md) |
| 14 | Pub-Sub System | Medium | [Solution](practice-problems/14-pub-sub.md) |
| 15 | Meeting Scheduler | Medium | [Solution](practice-problems/15-meeting-scheduler.md) |
| 16 | Task Scheduler | Medium | [Solution](practice-problems/16-task-scheduler.md) |
| 17 | Movie Ticket Booking (BookMyShow) | Hard | [Solution](practice-problems/17-movie-ticket-booking.md) |
| 18 | Chess | Hard | |
| 19 | Ride-Sharing Service (Uber) | Hard | |
| 20 | Food Delivery Service (Swiggy) | Hard | |
| 21 | Online Shopping System (Amazon) | Hard | |

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
