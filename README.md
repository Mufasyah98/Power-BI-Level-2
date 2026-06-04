https://mufasyah-my.sharepoint.com/:x:/g/personal/fakhrul_syahmi_mufasyah_onmicrosoft_com/IQDRGhCrBuWiQ56yxuaXH0yCAagJgo_rjmRV8b5k_bmxBSI?e=zkJPeo

# RetailMart Power BI Training Dataset

## Overview

This repository contains a complete business-oriented dataset designed for Microsoft Power BI training, workshops, bootcamps, and self-learning projects.

The dataset simulates a retail company called **RetailMart**, operating multiple stores across Malaysia through physical outlets, online channels, and mobile applications.

The objective is to provide realistic business scenarios for participants to practice:

* Data Modelling
* Power Query
* DAX Calculations
* Dashboard Development
* Business Analytics
* Executive Reporting
* Data Storytelling

---

# Business Scenario

RetailMart is a growing retail company with stores across multiple regions in Malaysia.

Management requires a Business Intelligence solution to answer critical business questions such as:

* Which stores generate the highest sales?
* Which products contribute the most profit?
* What are the sales trends over time?
* Which customer segments are the most valuable?
* Which products experience the highest return rates?
* How can management improve profitability?

Participants will act as Data Analysts and develop interactive Power BI dashboards to support business decision-making.

---

# Dataset Structure

## Fact Tables

### FactSales

Main transaction table containing sales records.

| Column      | Description           |
| ----------- | --------------------- |
| SalesID     | Unique transaction ID |
| OrderDate   | Transaction date      |
| CustomerID  | Customer identifier   |
| ProductID   | Product identifier    |
| StoreID     | Store identifier      |
| Quantity    | Units sold            |
| UnitPrice   | Product selling price |
| Discount    | Discount amount       |
| SalesAmount | Total sales amount    |
| CostAmount  | Product cost          |
| GrossProfit | Sales - Cost          |

---

### FactReturns

Contains returned product transactions.

| Column       | Description               |
| ------------ | ------------------------- |
| ReturnID     | Return transaction ID     |
| SalesID      | Related sales transaction |
| ProductID    | Product returned          |
| StoreID      | Store location            |
| ReturnDate   | Return date               |
| ReturnReason | Reason for return         |
| ReturnAmount | Amount returned           |

---

## Dimension Tables

### DimCustomer

Customer master information.

| Column         | Description               |
| -------------- | ------------------------- |
| CustomerID     | Customer identifier       |
| CustomerName   | Customer name             |
| Gender         | Male/Female               |
| Age            | Customer age              |
| State          | Customer location         |
| LoyaltySegment | Customer loyalty category |

---

### DimProduct

Product master information.

| Column      | Description         |
| ----------- | ------------------- |
| ProductID   | Product identifier  |
| ProductName | Product name        |
| Category    | Product category    |
| SubCategory | Product subcategory |
| Brand       | Product brand       |

---

### DimStore

Store information.

| Column    | Description       |
| --------- | ----------------- |
| StoreID   | Store identifier  |
| StoreName | Store name        |
| Region    | Sales region      |
| State     | Store state       |
| StoreType | Physical / Online |

---

### DimDate

Calendar table used for time intelligence analysis.

| Column    | Description   |
| --------- | ------------- |
| Date      | Calendar date |
| Year      | Year          |
| Quarter   | Quarter       |
| Month     | Month         |
| MonthName | Month name    |
| Weekday   | Day name      |

---

# Recommended Data Model

Star Schema Structure

```text
                 DimDate
                    |
                    |
DimCustomer --- FactSales --- DimProduct
                    |
                    |
                 DimStore

FactReturns --> DimProduct
FactReturns --> DimStore
```

---

# Training Modules

## Module 1: Data Modelling

Participants will learn:

* Star Schema Design
* Fact vs Dimension Tables
* Relationship Management
* Active vs Inactive Relationships
* Filter Direction
* Model Optimization

---

## Module 2: Power Query

Participants will learn:

* Data Cleaning
* Data Transformation
* Merge Queries
* Append Queries
* Custom Columns
* Text Functions
* Number Functions
* Date Functions

---

## Module 3: DAX Fundamentals

Participants will create:

```DAX
Total Sales
Total Gross Profit
Total Transactions
Average Order Value
Profit Margin %
```

---

## Module 4: Time Intelligence

Participants will create:

```DAX
Sales YTD
Sales MTD
Sales QTD
Previous Year Sales
Sales Growth %
```

---

## Module 5: Executive Dashboard

Build:

* KPI Dashboard
* Sales Trend Analysis
* Store Performance Analysis
* Product Performance Analysis
* Customer Analysis

---

## Module 6: Advanced Analytics

Build:

* Dynamic Ranking
* Top N Analysis
* Drill Through Pages
* Tooltip Pages
* Bookmark Navigation
* Executive Reporting Dashboard

---

# Case Studies

### Case Study 1

Executive Sales Performance Dashboard

### Case Study 2

Store Performance Analysis

### Case Study 3

Product Profitability Analysis

### Case Study 4

Customer Segmentation Analysis

### Case Study 5

Return Analysis Dashboard

### Case Study 6

Management Executive Dashboard

---

# Learning Outcomes

Upon completion, participants will be able to:

* Design a professional Power BI data model
* Develop advanced DAX measures
* Create business-focused dashboards
* Analyze sales and profitability
* Build executive-level reports
* Deliver actionable business insights

---

# Software Requirements

* Microsoft Power BI Desktop (Latest Version)
* Microsoft Excel
* Windows 10 / Windows 11

---

# Target Audience

* Business Analysts
* Data Analysts
* Executives
* Managers
* Finance Professionals
* Operations Teams
* Students learning Business Intelligence

---

# Author

**Fakhrul Syahmi**

Data Analytics Consultant | Power BI Trainer | Microsoft Excel Specialist | AI & Business Intelligence Trainer

Training Areas:

* Microsoft Power BI
* Microsoft Excel
* Power Platform
* Data Analytics
* AI for Productivity
* Business Intelligence

---

# License

This dataset is provided for educational and training purposes only.
