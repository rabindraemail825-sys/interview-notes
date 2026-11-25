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

A curated set of commonly asked problems. The levels and times are a suggested study order, not an official ranking.

| Level | Questions | Time per question |
|---|---|---|
| Basic | 1-5 | 30 min |
| Easy | 6-10 | 45 min |
| Medium | 11-15 | 60 min |
| Hard | 16-20 | 60 min |

### Basic

Core classes, clean state and simple rules.

#### 1. Tic-Tac-Toe

- [ ] Solved
- **Interviewer:** "Design a two-player Tic-Tac-Toe game."
- **What is tested:** entity modelling, win detection
- **Follow-up:** "How would you support an N x N board and check a win in O(1)?"

#### 2. Snake and Ladder

- [ ] Solved
- **Interviewer:** "Design a Snake and Ladder game for multiple players."
- **What is tested:** turn handling, separation of responsibilities
- **Follow-up:** "How would you add new dice rules without changing the game loop?"

#### 3. Vending Machine

- [ ] Solved
- **Interviewer:** "Design a vending machine that accepts money and dispenses items."
- **What is tested:** State pattern, invalid transitions
- **Follow-up:** "What happens if the machine cannot return exact change?"

#### 4. Logging Framework

- [ ] Solved
- **Interviewer:** "Design a logging library with levels and multiple outputs."
- **What is tested:** Strategy, Chain of Responsibility, Singleton trade-offs
- **Follow-up:** "How would you log asynchronously from many threads?"

#### 5. LRU Cache

- [ ] Solved
- **Interviewer:** "Design a fixed-capacity cache that evicts the least recently used key."
- **What is tested:** hash map with doubly linked list, O(1) operations
- **Follow-up:** "How would you make it thread-safe and support other eviction policies?"

### Easy

Several related classes and one or two design patterns.

#### 6. Parking Lot

- [ ] Solved
- **Interviewer:** "Design a multi-floor parking lot for different vehicle types."
- **What is tested:** class relationships, Strategy for pricing and spot allocation
- **Follow-up:** "How do you stop two entry gates from assigning the same spot?"

#### 7. ATM

- [ ] Solved
- **Interviewer:** "Design an ATM for balance enquiry, withdrawal and deposit."
- **What is tested:** State pattern, Chain of Responsibility for cash dispensing
- **Follow-up:** "What if cash dispensing fails after the account is debited?"

#### 8. Library Management System

- [ ] Solved
- **Interviewer:** "Design a system to search, borrow, reserve and return books."
- **What is tested:** book vs copy modelling, associations
- **Follow-up:** "How would you handle reservations and late fines?"

#### 9. Notification System

- [ ] Solved
- **Interviewer:** "Design a service that sends email, SMS and push notifications."
- **What is tested:** Factory, Strategy, Open/Closed Principle
- **Follow-up:** "How would you retry failures without sending duplicates?"

#### 10. Hotel Management System

- [ ] Solved
- **Interviewer:** "Design room search, booking, check-in and checkout for a hotel."
- **What is tested:** booking lifecycle, date-range availability
- **Follow-up:** "How do you prevent double booking of a room?"

### Medium

Scheduling, algorithms, extensibility and concurrency.

#### 11. Elevator System

- [ ] Solved
- **Interviewer:** "Design the control system for multiple elevators in a building."
- **What is tested:** State, Strategy for scheduling
- **Follow-up:** "How would you swap the scheduling algorithm at peak hours?"

#### 12. Splitwise

- [ ] Solved
- **Interviewer:** "Design an expense-sharing app with equal, exact and percentage splits."
- **What is tested:** polymorphic split types, balance tracking
- **Follow-up:** "How would you minimise the number of settlement payments?"

#### 13. Rate Limiter

- [ ] Solved
- **Interviewer:** "Design a rate limiter that restricts requests per user."
- **What is tested:** token bucket vs sliding window, thread safety
- **Follow-up:** "What changes if the limit must hold across many servers?"

#### 14. Pub-Sub System

- [ ] Solved
- **Interviewer:** "Design an in-memory publish-subscribe system with topics."
- **What is tested:** Observer, producer-consumer
- **Follow-up:** "How do you handle a slow subscriber and keep message order?"

#### 15. Meeting Scheduler

- [ ] Solved
- **Interviewer:** "Design a system to book meeting rooms and invite attendees."
- **What is tested:** interval conflicts, notifications
- **Follow-up:** "How would you support recurring meetings?"

### Hard

Large scope, so agree on what to leave out first.

#### 16. Movie Ticket Booking (BookMyShow)

- [ ] Solved
- **Interviewer:** "Design movie search, seat selection and ticket booking."
- **What is tested:** seat locking, concurrency, payment flow
- **Follow-up:** "Two users pick the same seat at once. What happens?"

#### 17. Chess

- [ ] Solved
- **Interviewer:** "Design a two-player chess game."
- **What is tested:** piece polymorphism, move validation, Command for undo
- **Follow-up:** "How would you handle check, castling and undo?"

#### 18. Ride-Sharing Service (Uber)

- [ ] Solved
- **Interviewer:** "Design rider requests, driver matching, trips and fares."
- **What is tested:** Strategy for matching and pricing, trip states
- **Follow-up:** "How do you stop one driver from being assigned two rides?"

#### 19. Food Delivery Service (Swiggy)

- [ ] Solved
- **Interviewer:** "Design restaurant search, ordering and delivery assignment."
- **What is tested:** order state machine, Observer for status updates
- **Follow-up:** "What happens if no delivery partner accepts the order?"

#### 20. Online Shopping System (Amazon)

- [ ] Solved
- **Interviewer:** "Design product catalogue, cart, checkout and order tracking."
- **What is tested:** inventory consistency, payment abstraction
- **Follow-up:** "How do you avoid overselling the last item?"

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
