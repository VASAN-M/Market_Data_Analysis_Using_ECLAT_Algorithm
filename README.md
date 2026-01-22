# Market Basket Analysis using ECLAT Algorithm

This project performs **Market Basket Analysis** using the **ECLAT
(Equivalence Class Transformation)** algorithm to identify frequent
itemsets from transactional data. ECLAT is an efficient alternative to
Apriori that uses a vertical data format to compute itemset support.

---

## Overview

Market Basket Analysis is commonly used in retail analytics to discover
frequently co-occurring items in customer transactions.  
In this project, the ECLAT algorithm is applied to transactional data to
extract frequent item combinations based on minimum support thresholds.

---

## Dataset
- File: `Market_Basket_Optimisation.csv`
- Each row represents a transaction
- Each column represents an item in the transaction
- Empty or unused entries are represented as missing values

---

## Workflow

### 1. Data Loading and Inspection
- Loaded the dataset using pandas
- Inspected:
  - Dataset structure and data types
  - Value distribution across columns
  - Summary statistics
  - Missing values

---

### 2. ECLAT Algorithm
- Used the `pyECLAT` library to implement the ECLAT algorithm
- Converted transactional data into a vertical format internally
- Extracted frequent itemsets using the following parameters:
  - Minimum support: `0.02`
  - Minimum itemset size: `1`
  - Maximum itemset size: `3`
  - Item separator: `&`

---

### 3. Frequent Itemset Extraction
- Retrieved:
  - Frequent itemset indexes
  - Corresponding support values
- Printed itemsets and their supports for analysis

---

## Libraries Used
- pandas
- numpy
- pyECLAT
- matplotlib

---

## How to Run

### 1. Install dependencies
```bash
pip install pandas numpy pyECLAT matplotlib
