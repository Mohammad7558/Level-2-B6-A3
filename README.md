# Vehicle Rental System  
**SQL Database Assignment**

---

## Overview
The Vehicle Rental System is a relational database–based project designed to model the core operations of a real-world vehicle rental business. The system focuses on managing users, vehicles, and bookings while maintaining data integrity and supporting analytical queries.

This project demonstrates practical SQL usage for handling rental workflows, availability tracking, and historical data analysis.

---

## System Features
- User management with role-based distinction (Admin and Customer)
- Vehicle inventory management with availability tracking
- Booking and rental history management
- Query-based reporting for business insights

---

## Database Schema

### Tables

#### 1. Users
Stores information about system users.
- User ID (Primary Key)
- Name
- Contact details
- Role (Admin / Customer)

#### 2. Vehicles
Stores information about rental vehicles.
- Vehicle ID (Primary Key)
- Make
- Model
- Vehicle type
- Availability status

#### 3. Bookings
Manages rental transactions.
- Booking ID (Primary Key)
- User ID (Foreign Key)
- Vehicle ID (Foreign Key)
- Rental start date
- Rental end date
- Booking status

---

## Relationships
- One user can create multiple bookings (One-to-Many)
- One vehicle can be booked multiple times (One-to-Many)
- Each booking is associated with exactly one user and one vehicle

These relationships are enforced using foreign key constraints to ensure referential integrity.

---

## SQL Concepts Applied
This project applies several important SQL concepts, including:

- **INNER JOIN**  
  Used to retrieve related data across Users, Vehicles, and Bookings tables.

- **NOT EXISTS**  
  Applied to identify records based on the absence of related data.

- **WHERE Clause**  
  Filters records according to specific conditions.

- **GROUP BY & HAVING**  
  Used for aggregation and conditional filtering of grouped data.

- **Primary and Foreign Keys**  
  Ensure data consistency and enforce relationships between tables.

---

## Project Files
- `queries.sql`  
  Contains all SQL queries including inserts, joins, filters, and analytical queries.

- `README.md`  
  Project documentation describing the database structure and logic.

- **Entity Relationship Diagram (ERD)**  
  Visual representation of the database schema and relationships  
  https://dbdiagram.io/d/69496b5661d95806cf350adb

---

## Author
**Mohammad Bin Amin**  
Software Developer
