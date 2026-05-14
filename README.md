#  <img src="https://upload.wikimedia.org/wikipedia/en/d/d3/Starbucks_Corporation_Logo_2011.svg" width="40"/> Starbucks Daily Sales Analysis Dashboard
## 📌 Project Description
The Starbucks Daily Sales Analysis Dashboard is a complete end-to-end Business Intelligence project developed using SQL Server and Power BI.
The project focuses on analyzing Starbucks sales transactions to generate meaningful business insights related to customer behavior, sales performance, order trends, and product analysis.

In this project:
- Raw data was first stored and managed in SQL Server
- SQL queries were used for data extraction and preprocessing
- Data was imported into Power BI
- Data modeling and relationships were created
- DAX measures were written for KPI calculations
- Interactive dashboards were designed for visual analysis

This dashboard helps businesses monitor daily operations and make data-driven decisions.

## 🎯 Project Objectives
The primary objectives of this project are:
- Analyze daily sales performance
- Track total revenue and orders
- Monitor customer purchasing behavior
- Identify peak sales hours
- Analyze product demand
- Measure average order value
- Build an interactive and professional dashboard

## 🛠️ Tech Stack
- SQL Server – Data storage & querying
- Power BI – Dashboard creation & visualization
- DAX – Measures and calculations
- Power Query – Data cleaning & transformation
- Excel/CSV Dataset

## 📂 Dataset Information
The project contains:
- Sales Transactions
- Customer Details
- Product/Items Information
- Time/Calendar Data

 The SQL database tables were imported into Power BI using SQL Server connection.

## ⚙️ SQL Implementation
 SQL Tasks Performed :
- Created Starbucks database
- Created relational tables
- Inserted customer, item, and sales data
- Analyzed revenue and sales trends
- Prepared data for Power BI reporting

## 📝 SQL Code Included
The project contains SQL scripts for:
- Database creation
- Table creation
- Data insertion
- Sales analysis queries

```sql
-- Create Database
CREATE DATABASE Starbucks;
USE Starbucks;

-- Customers Table
CREATE TABLE customers (
    customer_id INT PRIMARY KEY,
    customer_name TEXT,
    customer_email TEXT,
    customer_phone TEXT,
    customer_age INT,
    customer_gender TEXT
);

-- Items Table
CREATE TABLE items (
    id INT PRIMARY KEY,
    item TEXT,
    calories INT,
    fat FLOAT,
    carb INT,
    fiber INT,
    protein INT,
    type TEXT
);

-- Sales Table
CREATE TABLE sales (
    transaction_id VARCHAR(500) PRIMARY KEY,
    store_id INT,
    datetime DATETIME,
    customer_id INT,
    item_id INT,
    quantity INT,
    price FLOAT,
    total_amount FLOAT,
    payment_mode TEXT,
    customer_type TEXT
);
```
## 🔗 Data Modeling
Relationships were created between:
- sales ↔ customers
- sales ↔ items
- sales ↔ calendar

This star schema model improves reporting performance and supports accurate analysis.

## 📊 Dashboard Features
### 🏠 Home Page
- Interactive landing page
- Navigation buttons
- Professional dashboard design

### 📈 Overview Dashboard
This page displays key KPIs such as:
#### KPIs :
- Total Orders
- Total Customers
- Total Revenue
- Total Quantity Sold
#### Charts & Visuals :
- Average Order Amount by Hour
- Total Amount by Hour
- Total Quantity by Hour
#### Insights :
- Identifies busiest sales hours
- Tracks customer spending behavior
- Shows sales trends throughout the day
  
### 📋 Details Dashboard
Provides detailed transaction-level analysis including:
- Customer details
- Product purchased
- Quantity sold
- Payment mode
- Order value

## 📷 Dashboard Preview
### Home Page
<img width="1337" height="797" alt="Starbucks Dashboard(Home page)" src="https://github.com/user-attachments/assets/241f1513-c709-4f94-bb71-b98827aaa5ae" />

### Overview Analysis
<img width="1348" height="792" alt="Starbucks Dashboard(Overview Page)" src="https://github.com/user-attachments/assets/0ae235f5-ad0f-467c-8087-9894bf1c59e8" />

### Details Analysis
<img width="1347" height="793" alt="Starbucks Dashboard(Details Page)" src="https://github.com/user-attachments/assets/71b35b7f-a696-4c21-ad41-ca00392286a2" />

### Model View
<img width="1492" height="787" alt="Starbucks Dashboard(Model view)" src="https://github.com/user-attachments/assets/a1a991e4-3afc-4b6f-ab64-1f189b3c2e37" />

## 💡 Business Insights Derived
- Identified peak sales hours
- Analyzed customer purchasing patterns
- Tracked revenue performance
- Monitored product demand trends
