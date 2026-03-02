# Pakistan Tourism Management System (SQL & Python DBMS)

A fully normalized Database Management System (DBMS) developed to manage tourism operations including tourists, bookings, packages, accommodations, guides, payments, transportation, and cultural events.

This project demonstrates advanced database design, normalization to 3NF, SQL query development, and Python GUI integration.

---

##  Project Overview

The **Pakistan Tourism Management System (PTMS)** is designed to:

- Manage tourist records
- Handle bookings and travel packages
- Store accommodation and transportation details
- Maintain guide assignments
- Record payments and tourist feedback
- Generate unified tourism reports using SQL Views

The system ensures structured, scalable, and efficient data management.

---

##  Database Design

###  Database Structure

- 17 Interconnected Tables
- Primary Key & Foreign Key Constraints
- Junction Tables for Many-to-Many Relationships
- Fully Normalized up to **Third Normal Form (3NF)**

---

###  Main Tables

- Tourists  
- TouristPackages  
- Bookings  
- PackagePricing  
- Destinations  
- Guides  
- GuideDestinations  
- Accommodations  
- TouristFeedback  
- Transportation  
- TouristPayments  
- CulturalEvents  
- EventCosts  
- EmergencyContacts  
- ContactNames  
- TouristGroups  
- RoomBookings  

---

##  Normalization Process

The database was normalized to eliminate redundancy and ensure data integrity.

###  First Normal Form (1NF)
- Removed multi-valued attributes
- Split ContactInfo and TouristSpots into atomic values

###  Second Normal Form (2NF)
- Removed partial dependencies
- Created **PackagePricing** table
- Created **GuideDestinations** junction table

### Third Normal Form (3NF)
- Removed transitive dependencies
- Separated **EventCosts** table
- Created **ContactNames** table

---

## SQL Features Implemented

- Table creation with constraints
- Composite Primary Keys
- Foreign Key Relationships
- Data insertion queries
- Advanced JOIN queries
- Custom SQL View

###  Custom View

sql
CREATE VIEW FullTourismView AS
-- Complex JOIN Query Combining All Major Tables

The view combines tourist, booking, package, accommodation, guide, payment, and event information into a unified report.

---

### Python Portal (Frontend)
 Technology Used

Python

Tkinter (GUI Framework)

SQL Database Backend

 
---

## Portal Features

Add new records (Create)

View existing data (Read)

Modify records (Update)

Remove records safely (Delete)

Input validation

Foreign key constraint handling

Error handling with user-friendly messages

Dynamic SQL query execution


---

## CRUD Operations

✔ Create – Add new records with validation
✔ Read – Retrieve data using SELECT queries with JOINs
✔ Update – Modify records securely
✔ Delete – Remove records with confirmation prompts

 
---

## Error Handling

Input validation checks

Database constraint management

Foreign key violation handling

Safe deletion confirmations

 
---

## Sample Data

The system includes sample data for:

Tourists

Travel Packages

Bookings

Guides

Accommodations

Payments

Cultural Events

This allows full testing of database relationships and portal functionality.

 
---

## Project Files Included

SQL Script (Before Normalization)

SQL Script (After 3NF Normalization)

ER Diagram

Python GUI Source Code

Database Schema

Project Report

 
---

## Academic Purpose

This project was developed as part of a Database Management Systems course to demonstrate:

Practical relational database design

Normalization techniques (1NF → 3NF)

SQL constraints and joins

Backend integration with a GUI application

Real-world tourism management simulation
