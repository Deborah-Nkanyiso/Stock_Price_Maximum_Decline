# Stock Price Maximum Decline Analyzer

A Java program that analyzes stock price behavior using a trigonometric price model and calculates the **maximum decline** in price over a given period for multiple stocks.

**Author:** DN MBOYI  
**Student Number:** 222019179  
**Assignment:** Custom ArrayList + Stock Analysis  
**Course:** CSC03B3 (Data Structures / Java Programming)

---

## Project Description

This application:
- Reads a collection of `Stock` objects from a binary database file (`stock.db`)
- Uses a mathematical model to simulate daily stock prices:
- price(k) = p × (sin(a×k + b) + cos(c×k + d) + 2)

- Calculates the **maximum decline** (biggest drop from any peak) for each stock
- Demonstrates a fully custom generic `ArrayList` implementation with iterator support

---

## Features

### Core Functionality
- Custom generic `ArrayList<T>` with dynamic resizing
- Two resizing strategies: **Incremental (+1)** and **Doubling**
- Full `List` interface implementation (`add`, `remove`, `get`, `set`)
- Custom `Iterator` for the ArrayList (`ArrayListIterator`)
- Binary file deserialization using `ObjectInputStream`
- Mathematical stock price simulation
- Maximum decline calculation for each stock

### Exception Handling
- `ArrayListException` (RuntimeException) for invalid indices

---

## Files Included

- `Main.java` – Main program and stock processing logic
- `ArrayList.java` – Custom generic ArrayList implementation
- `ArrayListIterator.java` – Iterator for ArrayList
- `List.java` – List interface
- `Stock.java` – Stock model class (Serializable)
- `ArrayListException.java` – Custom exception

---

## Technologies Used

- **Java Generics**
- **Custom Data Structure** (`ArrayList`)
- **Iterator Pattern**
- **Object Serialization / Deserialization**
- **Mathematical Modeling** (trigonometric functions)
- **File I/O** (Binary `.db` file)

---

## How to Run

1. Ensure the database file `data/stock.db` exists in the correct path
2. Compile all Java files:
 ```bash
 javac *.java
