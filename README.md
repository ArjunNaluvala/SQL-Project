# Grocery Store Management System

# Overview

The **Grocery Store Management System** is a complete relational database project designed using **MySQL** to simulate real-world retail store operations.

The project focuses on managing customers, products, suppliers, employees, orders, and sales transactions while generating business insights using advanced SQL queries.

This project demonstrates strong understanding of:

* Relational Database Design
* SQL Query Optimization
* Business Analytics
* Retail Sales Analysis
* Data Modeling
* Aggregation & Reporting
* Foreign Key Relationships

# Business Problem

Retail businesses generate large volumes of transactional data daily. Managing customer orders, inventory, suppliers, and sales reporting manually becomes inefficient and error-prone.

This project solves the problem by:

* Designing a normalized relational database
* Managing transactional operations efficiently
* Generating analytical business reports
* Identifying revenue trends and customer insights
* Supporting data-driven business decisions

# Objectives

* Design a normalized retail database system
* Implement relational schema architecture
* Build customer and order management workflows
* Perform business analytics using SQL
* Generate sales and revenue insights
* Analyze supplier and employee performance

# Database Architecture

## Tables Included

| Table Name    | Description                         |
| ------------- | ----------------------------------- |
| Customers     | Stores customer information         |
| Products      | Product details and pricing         |
| Orders        | Customer order records              |
| Order_Details | Transaction-level order information |
| Suppliers     | Supplier information                |
| Categories    | Product categories                  |
| Employees     | Employee management                 |

# Database Relationships

* One-to-Many Relationships
* Foreign Key Constraints
* CASCADE Rules
* Referential Integrity
* Normalized Schema Design

# SQL Concepts Used

## Core SQL

* SELECT
* WHERE
* ORDER BY
* GROUP BY
* HAVING
* DISTINCT

## Advanced SQL

* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* Subqueries
* CASE WHEN
* Aggregate Functions
* Date Functions
* Nested Queries

## Aggregations

* SUM()
* AVG()
* COUNT()
* MAX()
* MIN()

# Database Features

* 7 Relational Tables
* 6 Foreign Key Constraints
* Normalized Database Design
* Transaction Management
* Revenue Reporting
* Business Intelligence Queries
* Customer Analytics
* Supplier Performance Analysis

# Analysis Categories

## 1. Customer Insights

* Top customers by revenue
* Customer purchase frequency
* Spending analysis
* Order history tracking

## 2. Product Performance

* Best-selling products
* Product category analysis
* Revenue contribution by products
* Inventory movement insights

## 3. Sales Trends

* Monthly revenue analysis
* Daily order trends
* Weekday vs weekend sales
* Peak business periods

## 4. Supplier Contribution

* Highest revenue suppliers
* Supplier product contribution
* Supplier performance tracking

## 5. Employee Performance

* Employee order handling
* Productivity analysis
* Operational efficiency tracking

# Sample SQL Queries

## Top Customers by Revenue

```sql
SELECT customer_name,
       SUM(total_amount) AS total_revenue
FROM orders
GROUP BY customer_name
ORDER BY total_revenue DESC;
```

---

## Best-Selling Products

```sql
SELECT product_name,
       SUM(quantity) AS total_quantity_sold
FROM order_details
GROUP BY product_name
ORDER BY total_quantity_sold DESC;
```

---

## Monthly Revenue Trend

```sql
SELECT MONTH(order_date) AS month,
       SUM(total_amount) AS revenue
FROM orders
GROUP BY MONTH(order_date)
ORDER BY month;
```

# Key Business Insights

* Identified top revenue-generating customers
* Determined highest-selling product categories
* Analyzed monthly revenue growth trends
* Identified supplier contribution patterns
* Evaluated employee operational performance
* Compared weekday vs weekend sales behavior

# Business Impact

This system helps businesses:

* Improve operational efficiency
* Track revenue performance
* Understand customer behavior
* Monitor inventory movement
* Support data-driven decisions
* Optimize supplier relationships

# Project Workflow

```text
Database Design
      ↓
Table Creation
      ↓
Relationship Setup
      ↓
Data Insertion
      ↓
SQL Query Development
      ↓
Business Analysis
      ↓
Insight Generation
```

# Tools & Technologies

* MySQL
* SQL
* Relational Database Design
* Data Analysis
* Business Intelligence

# Future Improvements

* Inventory Management Module
* Billing Automation
* Real-Time Dashboard Integration
* Stored Procedures
* Triggers
* User Authentication System
* Power BI Dashboard Integration

# Skills Demonstrated

* SQL Query Writing
* Relational Database Design
* Business Analytics
* Data Modeling
* Aggregation & Reporting
* Data Analysis
* Problem Solving
