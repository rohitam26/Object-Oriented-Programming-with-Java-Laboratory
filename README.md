# Object-Oriented Programming with Java Laboratory

[![Java](https://img.shields.io/badge/Language-Java%2017%2F21-ED8B00.svg)](https://www.oracle.com/java/)
[![OOP](https://img.shields.io/badge/Paradigm-OOP-43853D.svg)](#)
[![JDBC](https://img.shields.io/badge/Database-JDBC%20%7C%20MySQL-00758F.svg)](https://dev.mysql.com/doc/connector-j/en/)
[![License](https://img.shields.io/badge/License-Academic-lightgrey.svg)](#)

## 1. Project Title
**Object-Oriented Programming with Java Laboratory: OOP Principles, Modern Java Features, and JDBC Database Application**

## 2. Project Overview
This repository contains the complete academic laboratory coursework and capstone project for **Object-Oriented Programming using Java**, completed as part of the B.E. Artificial Intelligence and Machine Learning curriculum at Rajalakshmi Engineering College.

The repository spans progressive OOP principles—encapsulation, inheritance hierarchies, runtime polymorphism, abstract classes, interfaces, robust exception handling, Java Collections Framework, and modern Java Lambda expressions. It culminates in a full backend database project: an **Inventory Management System** engineered using **Java Database Connectivity (JDBC)** and MySQL.

---

## 3. Objectives
- Master fundamental object-oriented programming concepts: encapsulation, inheritance, polymorphism, and abstraction.
- Implement robust memory and reference management using constructors, method overloading/overriding, and the `this` and `super` keywords.
- Enforce interface-driven architecture and explore multiple inheritance through Java interfaces.
- Design resilient fault-tolerant systems using Java's structured exception handling mechanism (`try-catch-finally`, custom exceptions).
- Leverage modern functional programming features in Java, including Lambda expressions and stream pipelines.
- Build a persistent enterprise-style console application connecting Java applications to relational database backends via JDBC.

---

## 4. Key Features
- **Structured Progressive Curriculum**: 12 weeks of assessed laboratory modules progressing systematically from syntax fundamentals to advanced enterprise topics.
- **Pure OOP Architecture**: Real-world domain entities modeled with strict access controls, immutable patterns, and inheritance hierarchies.
- **Enterprise JDBC Project**: A production-grade `InventoryManagementSystem` integrating `java.sql.Connection`, `PreparedStatement`, `Statement`, and `ResultSet` with a MySQL database.
- **Fault-Tolerant Exception Handling**: Standardized recovery mechanisms and custom exception classes enforcing business constraints.
- **Collections Framework**: Practical implementations of dynamic memory collections (`ArrayList`, `HashMap`, `HashSet`, and `Iterators`).
- **Functional Java**: Concise data transformations using Lambda expressions and functional interfaces.

---

## 5. Technologies Used
- **Programming Language**: Java (JDK 17 / 21 LTS)
- **Database Backend**: MySQL Server 8.0+
- **Connectivity Framework**: Java Database Connectivity (JDBC), MySQL Connector/J (`mysql-connector-j-8.x.jar`)
- **Core APIs**: `java.lang`, `java.util`, `java.io`, `java.sql`, `java.util.function`
- **Assessment Platform**: NeoColab Lab Evaluation Records (Rajalakshmi Engineering College)

---

## 6. Project Structure
```text
Object-Orientented-Programming-with-Java/
│
├── 241501168 Java record_week1.pdf    # Week 1: Java Basics, Scanner I/O, Conditionals, and Control Flow
├── 241501168 Java record_week2.pdf    # Week 2: Array Structures (1D/2D), String API & Text Manipulation
├── 241501168 Java record_week3.pdf    # Week 3: Class Architecture, Constructors, Overloading & 'this'
├── 241501168 Java record_week4.pdf    # Week 4: Encapsulation, Access Modifiers, and Package Structuring
├── 241501168 Java record_week5.pdf    # Week 5: Inheritance Hierarchies, Dynamic Method Dispatch & 'super'
├── 241501168 Java record_week6.pdf    # Week 6: Abstraction, Abstract Classes, and Interface Contracts
├── 241501168 Java record_week7.pdf    # Week 7: Structured Exception Handling & Custom Exceptions
├── 241501168 Java record_week8.pdf    # Week 8: Multithreading, Thread Synchronization & Concurrency
├── 241501168 Java record_week9.pdf    # Week 9: Java Collections Framework (Lists, Sets, Maps)
├── 241501168 Java record_week10.pdf   # Week 10: File I/O, Byte/Character Streams & Serialization
├── 241501168 Java record_project.pdf  # Week 11 Capstone: JDBC-MySQL Inventory Management System
├── 241501168 Java record_week12.pdf   # Week 12: Modern Java Features, Functional Interfaces & Lambdas
│
└── README.md
```

---

## 7. Installation and Prerequisites
### Prerequisites
- Java Development Kit (JDK 17 LTS or newer)
- MySQL Server (v8.0+)
- MySQL Connector/J driver

### Verifying Java Environment
```bash
java -version
javac -version
```

### MySQL Database Setup for Capstone Project
```sql
CREATE DATABASE ri_db;
USE ri_db;

CREATE TABLE items (
    item_id INT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    quantity INT NOT NULL,
    price DECIMAL(10, 2) NOT NULL
);
```

---

## 8. Execution Instructions
### Compiling and Running Standard Laboratory Programs
```bash
javac -d bin src/Week1Program.java
java -cp bin Week1Program
```

### Compiling and Executing the Capstone JDBC Project
```bash
javac -cp ".;mysql-connector-j-8.2.0.jar" -d bin InventoryManagementSystem.java
java -cp "bin;mysql-connector-j-8.2.0.jar" InventoryManagementSystem
```

---

## 9. Implementation and Methodology

| Module / Week | Technical Focus | Core Concepts Implemented | Practical Problem / Assignment |
|---|---|---|---|
| **Week 1** | Fundamentals & I/O | Standard input parsing, data types, primitive operators, loops | Control flow logic, math series |
| **Week 2** | Arrays & Strings | Matrix operations, string searching, immutable String vs StringBuilder | String transformations, array searching |
| **Week 3** | Class & Objects | Class blueprints, parameterized constructors, constructor chaining | Real-world entity modeling |
| **Week 4** | Encapsulation | Private data hiding, public accessors, package encapsulation | Account and banking models |
| **Week 5** | Inheritance | Base/Derived classes, method overriding, polymorphic behavior | Vehicle and Employee hierarchies |
| **Week 6** | Abstraction | Abstract methods, contract enforcement via interfaces | Shape renderers, Payment gateways |
| **Week 7** | Exception Handling | `try`, `catch`, `finally`, nested exceptions, custom checked exceptions | Input validators, transaction rollback |
| **Week 8** | Multithreading | `Runnable` interface, `Thread` extension, thread synchronization | Concurrent producer-consumer tasks |
| **Week 9** | Collections | `ArrayList`, `HashMap`, `HashSet`, sorting with `Comparable` | In-memory student & record management |
| **Week 10** | File I/O | Character streams (`FileReader`, `FileWriter`), `BufferedReader` | File persistence and text parsing |
| **Capstone (W11)** | **JDBC Database App** | `DriverManager`, `Connection`, `Statement`, `ResultSet`, SQL DML | **Inventory Management System (MySQL)** |
| **Week 12** | Modern Java | Functional interfaces, Lambda expressions `(params) -> expr` | Stream filtering, list aggregations |

---

## 10. Results and Outputs
- **Academic Evaluation**: Verified 100% completion across all evaluated coding problem test cases and MCQ assessments (Grade: 20/20 on Capstone).
- **Capstone Execution**: The `InventoryManagementSystem` connected successfully to the local MySQL server (`ri_db`), demonstrating robust transactional workflows:
  - Add Item: Successfully inserted item records into the relational table.
  - Restock Item: Dynamically updated stock levels based on input quantity.
  - Reduce Item: Verified inventory availability, rejecting requests exceeding stock limits.
  - Display Inventory: Iterated over `ResultSet` records to display formatted tabular data.

---

## 11. Screenshots and Visual Documentation
Complete academic records, source code listings, test case execution traces, and NeoColab evaluation metrics are documented within the corresponding weekly PDF records:
- `241501168 Java record_project.pdf`: Full source code and test run output for the JDBC project.
- `241501168 Java record_week1.pdf` through `week12.pdf`: Step-by-step problem statements, source solutions, and test case pass reports.

---

## 12. Learning Outcomes
- Developed strong fluency in object-oriented software engineering principles in Java.
- Mastered defensive programming practices with structured exception handling and input validation.
- Gained real-world backend engineering experience linking Java desktop applications to persistent relational databases via JDBC.
- Acquired familiarity with modern functional idioms introduced in modern Java versions.

---

## 13. Future Improvements
- Refactor the console interface of the Inventory Management System into a modern GUI using JavaFX.
- Migrate raw JDBC calls to Spring Data JPA / Hibernate ORM for declarative persistence.
- Package the application into an executable `.jar` file using Apache Maven or Gradle.

---

## 14. Author
**Rohita M**  
- **GitHub**: [@rohitam26](https://github.com/rohitam26)  
- **Roll Number**: 241501168  
- **Academic Program**: B.E. Artificial Intelligence and Machine Learning  
- **Institution**: Rajalakshmi Engineering College  
