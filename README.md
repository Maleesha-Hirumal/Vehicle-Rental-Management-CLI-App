# Vehicle Rental Management System

## CCS1303 - Object Oriented Programming

**Version:** 3.0
**Date:** 15 February 2026

---

## Project Overview

The Vehicle Rental Management System is a Java-based console application developed as a group project to demonstrate core Object-Oriented Programming (OOP) principles. The system allows users to manage vehicle rentals efficiently, including adding vehicles, renting, returning, and tracking income using a MySQL database.

This project was developed for academic purposes under the module **CCS1303 – Object Oriented Programming** at SLTC Research University.

---

## OOP Concepts Used

### Inheritance

* `Car`, `Bike`, and `Van` classes extend the abstract `Vehicle` class.

### Polymorphism

* A single `Vehicle` reference is used to handle multiple object types dynamically.

### Abstraction

* The `Vehicle` class is abstract and defines common behavior for all vehicles.

### Encapsulation

* All class attributes are private and accessed using getters and setters.

---

## Features

* Add new vehicles (Car, Bike, Van)
* View all available vehicles
* Rent vehicles with automatic cost calculation
* Return rented vehicles
* Search vehicles by ID
* Advanced search (Brand / Availability)
* Track total rental income
* MySQL database integration
* Simple login system (root/root)
* Console-based user interface

---

## Technologies Used

* Java (OOP)
* MySQL Database
* JDBC (MySQL Connector/J)
* IntelliJ IDEA

---

## System Requirements

### Required Software

* Java JDK (8 or above)
* IntelliJ IDEA (Recommended)
* MySQL Server
* MySQL Connector/J (JAR file included in `/lib` folder)

---

## Project Structure

```
Project
│
├── Vehicle.java
├── Car.java
├── Bike.java
├── Van.java
├── RentalApp.java
├── DatabaseManager.java
├── Features.java
│
└── lib
    └── mysql-connector-java-8.0.33.jar
```

---

## Installation Guide

### Step 1: Clone Repository

```bash
git clone <your-repository-url>
```

### Step 2: Open Project

* Open IntelliJ IDEA
* Click **Open Project**
* Select project folder

### Step 3: Add MySQL Connector

1. Press `Ctrl + Alt + Shift + S`
2. Go to **Modules**
3. Select **Dependencies**
4. Click **+ Add**
5. Choose **JARs or Directories**
6. Select:

   ```
   lib/mysql-connector-java-8.0.33.jar
   ```
7. Click **Apply → OK**

---

## Login Credentials

```
Username: root
Password: root
```

---

## Main Menu

```
1. Add a Vehicle
2. View All Vehicles
3. Rent a Vehicle
4. Return a Vehicle
5. Search Vehicle by ID
6. View Total Rental Income
7. Advanced Search & Filtering
8. Database Operations
9. Logout & Exit
```

---

## Sample Data

### Car Example

```
Vehicle ID: CAR001
Brand: Toyota
Model: Corolla
Seats: 5
Rate Per Day: Rs. 5000
```

### Bike Example

```
Vehicle ID: BIKE001
Brand: Yamaha
Model: R15
Engine Capacity: 150CC
Rate Per Day: Rs. 2000
```

---

## Assumptions

* Vehicle IDs are unique and case-insensitive
* All prices are in Sri Lankan Rupees (LKR)
* A vehicle must be available before renting
* A vehicle must be rented before returning
* Rental income is only increased, not decreased
* Single admin user system

---

## Validation Rules

* All numeric inputs must be greater than zero
* Duplicate vehicle IDs are not allowed
* Invalid inputs require re-entry

---

## Limitations

* No GUI (console-based only)
* No customer management system
* No rental history tracking
* No payment gateway integration
* No date/time tracking for rentals
* Single-user login system only

---

## Future Improvements

* Add customer management module
* Implement rental history tracking
* Add GUI using JavaFX or Swing
* Multi-user authentication system
* Generate reports (PDF/Excel)
* Add online booking system
* Improve security and encryption

---

## Team Members

| Name          | Role             |
| ------------- | ---------------- |
| H. Maleesha Hirumal     | Lead Developer   |
| Member 2 Name | Senior Developer |
| Member 3 Name | Developer        |

---

### Team Responsibilities

**Lead Developer**

* System design and architecture
* Project coordination
* Database integration (MySQL + JDBC)

**Senior Developer**

* Core functionality development
* OOP implementation support
* Final integration and testing
  
**Developer**

* Feature implementation
* UI/menu development
* Testing and bug fixing

---

## Academic Information

This project was developed as part of the **CCS1303 – Object Oriented Programming** module at SLTC Research University to demonstrate practical implementation of OOP concepts in Java.

---

## License

This project is for educational purposes only.
