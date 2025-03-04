# StatePropertyDb
**State Property Management Database**
**Overview**
This project is a centralized database system designed to streamline property data management for construction projects, real estate professionals, and regulatory authorities. The system enhances data organization, accessibility, and collaboration by integrating a structured PostgreSQL database with optimized queries for efficient data retrieval.

**Problem Statement**
Managing property data has traditionally relied on spreadsheets and manual processes, leading to data inconsistencies, inefficiencies, and limited accessibility. This project aims to:

Provide a dedicated database solution for managing property data efficiently.
Enhance data retrieval speed and query performance for large datasets.
Facilitate collaboration between developers, architects, contractors, and government authorities.
Key Features
✅ Structured Database Schema – Organizes property details, ownership history, transaction records, census data, and pricing information.
✅ Optimized Query Performance – Uses indexing, partitioning, and query optimization to reduce execution time.
✅ Regulatory Compliance – Facilitates tracking of ownership, deeds, and sales for legal and taxation purposes.
✅ Scalable Data Management – Supports large datasets while maintaining data integrity.

**Technologies Used**
Database: PostgreSQL
Query Optimization: Indexing, Hash Joins, Composite Keys
Tools: pgAdmin, SQL Triggers, PL/pgSQL Functions
Version Control: Git & GitHub
Database Schema & Tables
The project contains multiple normalized tables following Boyce-Codd Normal Form (BCNF) for optimal data organization:

Owner Info – Stores property owner details.
House Info – Captures house number, street, city, and zip code.
Deed Info – Manages property deed records.
Census Data – Provides demographic information for properties.
Property Details – Contains property class, total living area, and attributes.
Price Details – Stores land value, total value, and last sale price.
Link Table – Acts as a junction table linking ownership, deeds, pricing, and census data.
Sample Queries Implemented
Find all properties owned by a specific owner and their deed details.
Retrieve properties that changed ownership in the last year.
Identify properties within a certain ZIP code with land value above a given amount.
Find the most expensive property sale recorded.
Aggregate total property values owned by each owner.
Performance Optimization
To improve query execution time, the following optimizations were applied:

Indexing: Implemented on frequently queried columns (Owner_ID, SBL, Price_ID).
Partitioning: Reduced processing overhead by splitting large tables into manageable segments.
Query Optimization: Used hash joins, composite keys, and indexing to reduce query execution time by up to 40%.
