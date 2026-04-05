# 📊 Power BI Project: Electronics Sales Data

## 📌 Project Overview
This project walks through the complete Power BI workflow using a real-world **electronics sales dataset** containing messy and inconsistent data.

The goal is to **clean, transform, analyze, and visualize** the data to generate meaningful business insights for decision-making in an electronics retail business.

---

## 🎯 Objective
- Clean and standardize dirty sales data
- Perform data analysis using DAX
- Build a structured data model
- Create an interactive dashboard
- Develop a detailed Power BI report

---

## 🧹 Step 1: Data Cleaning

Data cleaning ensures accuracy, consistency, and usability of the dataset.

### ✅ Key Tasks

#### 1. Ensure Consistent Data Types
- Convert `OrderDate` → Date format  
- Convert `SalesAmount`, `Profit`, `ShippingCost` → Numeric  
- Remove invalid text values in numeric/date columns  

#### 2. Fix Spelling Errors
- Standardize product names (e.g., *Samsung Galaxy S21*)  
- Correct country names and customer emails  

#### 3. Handle Missing Values
- Identify null/blank values in:
  - Profit  
  - SalesAmount  
  - ShippingCost  
- Decide to:
  - Remove  
  - Replace (impute)  
  - Fill with defaults  

#### 4. Handle Invalid Entries
- Replace or clean entries like:
  - `"Anonymous"`
  - `"N/A"`
- Flag suspicious rows (e.g., missing customer in paid transactions)

#### 5. Standardize Formats
- Normalize currency values:
  - `USD`, `usd`, `US Dollar` → **USD**
- Ensure consistent date formats

---

## 📊 Step 2: Data Analysis

Use **DAX (Data Analysis Expressions)** to derive key insights.

### 📌 Key Measures

#### 1. Total Sales
```DAX
Total Sales = SUM(Sales[SalesAmount])

Profit Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[SalesAmount])) * 100

## PROJECT SOLUTIONs
**Data Cleaning**
* OrderDate is in Date data type
<img width="950" height="482" alt="image" src="https://github.com/user-attachments/assets/a85b63c0-7567-4d4f-bfba-901ff12a5e9a" />



