# Vehicle Booking System - Database Queries

## Project Overview

This project contains SQL queries for a **Vehicle Booking System** database. The system manages vehicle rentals, customer bookings, and vehicle inventory through a relational database structure.

---

## Database Structure

### Tables

1. **users** - Customer information
   - `user_id` - Unique customer identifier
   - `name` - Customer name

2. **vehicle** - Vehicle inventory
   - `vehicle_id` - Unique vehicle identifier
   - `name` - Vehicle name
   - `type` - Vehicle type (e.g., 'car', 'truck', 'van')
   - `status` - Current status ('available', 'booked', 'maintenance')

3. **bookings** - Booking records
   - `booking_id` - Unique booking identifier
   - `user_id` - Reference to customer (foreign key)
   - `vehicle_id` - Reference to vehicle (foreign key)
   - `start_date` - Booking start date
   - `end_date` - Booking end date
   - `total_cost` - Booking cost

---

## SQL Queries Overview

This project includes 4 main SQL queries for different business purposes:

### 1. **Get Complete Booking Information**
Retrieves all bookings with customer and vehicle details.
- **Use Case**: Booking reports, customer history, administrative overview
- **Tables**: bookings, users, vehicle
- **Type**: JOIN query with multiple tables

### 2. **Find Vehicles with No Bookings**
Identifies unused vehicles in the inventory.
- **Use Case**: Inventory management, identifying idle assets
- **Tables**: vehicle, bookings
- **Type**: NOT EXISTS subquery

### 3. **Find Available Car Vehicles**
Lists all cars currently available for booking.
- **Use Case**: Customer search, availability checking
- **Tables**: vehicle
- **Type**: Simple WHERE filtering

### 4. **Get Vehicles with Multiple Bookings**
Shows popular vehicles with more than 2 bookings.
- **Use Case**: Analytics, identifying high-demand vehicles
- **Tables**: bookings, vehicle
- **Type**: GROUP BY aggregation with HAVING clause

---

## Files in This Project

- **queries.sql** - All SQL queries used in the system
- **QUERIES_EXPLANATION.md** - Detailed explanation of each query
- **README.md** - This file

---

## Key SQL Concepts

- **INNER JOIN** - Combining data from multiple tables
- **NOT EXISTS** - Filtering records based on non-existence in subqueries
- **GROUP BY** - Aggregating data by categories
- **HAVING** - Filtering aggregated results
- **COUNT()** - Counting records
- **WHERE & AND** - Conditional filtering
- **ORDER BY** - Sorting results

---

## How to Use

1. Open your database management system (MySQL, PostgreSQL, SQL Server, etc.)
2. Copy the desired query from `queries.sql`
3. Execute the query against your vehicle booking database
4. Refer to `QUERIES_EXPLANATION.md` for detailed information about each query

---

## Documentation

For **detailed explanations** of each query, including:
- Purpose and use cases
- Line-by-line code breakdown
- Expected results

See [QUERIES_EXPLANATION.md](QUERIES_EXPLANATION.md)

---

## Project Assignment

**Assignment #3** - Vehicle Booking System Database Queries

This project demonstrates practical SQL skills including:
- Multi-table joins
- Subqueries and filtering
- Aggregation and grouping
- Business logic implementation through queries

---

## Notes

- All queries are optimized for readability and performance
- Comments are provided in the explanation document
- Modify queries as needed for your specific database schema
- Ensure proper foreign key relationships exist before running queries

---

**Last Updated:** December 2025
