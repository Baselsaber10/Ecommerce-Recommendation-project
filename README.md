# Ecommerce Recommendation System

## Project Overview

This project focuses on building an Ecommerce Recommendation System using transactional retail data and association rule mining techniques.

The main objective is to discover relationships between products that are frequently purchased together and generate intelligent product recommendations.

The project was implemented using Python, Jupyter Notebook, Power BI, and Data Warehouse concepts.

---

## Dataset

The project uses the Online Retail Dataset which contains real transactional data from an ecommerce store.

Dataset features include:

- Invoice Number
- Product Code
- Product Description
- Quantity
- Invoice Date
- Unit Price
- Customer ID
- Country

The dataset represents transactional data where each row corresponds to a purchased product inside a customer transaction.

---

## Data Preprocessing

Several preprocessing steps were applied before building the recommendation system:

- Removing missing Customer IDs
- Removing cancelled invoices
- Removing invalid quantities and prices
- Cleaning duplicated records
- Transforming transactional data into basket format

---

## Data Warehouse Design

A Star Schema model was designed using:

### Fact Table
- Fact_Sales

### Dimension Tables
- Dim_Customers
- Dim_Products
- Dim_Time

The schema was implemented and visualized using Power BI.

---

## Recommendation Algorithms

Three association rule mining algorithms were implemented and compared:

### 1. Apriori
Generates frequent itemsets using candidate generation.

### 2. FP-Growth
Uses FP-Tree structure for faster frequent pattern mining.

### 3. ECLAT
Uses vertical transaction representation for efficient mining.

---

## Evaluation Metrics

The generated association rules were evaluated using:

- Support
- Confidence
- Lift
- Runtime Performance

---

## Results

The system successfully generated strong association rules between products.

Example recommendation:

```text
PINK REGENCY TEACUP AND SAUCER
→ GREEN REGENCY TEACUP AND SAUCER