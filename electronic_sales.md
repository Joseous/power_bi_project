# Power BI Project: Electronics Sales Data

## Objective
This project is designed to guide you through the entire Power BI workflow for a real-world scenario involving dirty sales data. You will clean, analyze, and model the data to create a dashboard and a detailed report with key business insights. The dataset contains inconsistent data, missing values, and currency discrepancies. The goal is to transform this data into useful information for decision-making in an electronics retail business.

## Step 1: Data Cleaning
Data cleaning ensures that the dataset is accurate and consistent.

- Ensure consistency in data types:
  Convert OrderDate and DeliveryDate to date format. Convert SalesAmount, Profit, and ShippingCost to numeric values. Remove invalid entries.

- Check for spelling errors:
  Standardize product names, country names, and customer emails. Ensure similar entries are uniform.

- Handle missing or incomplete data:
  Identify blanks in Profit, SalesAmount, and ShippingCost. Decide whether to remove, replace, or fill them.

- Handle pseudonyms and invalid entries:
  Clean entries such as "Anonymous" or "N/A". Flag suspicious records such as missing customer names in valid transactions.

- Ensure correct data formats:
  Standardize currencies (e.g., USD, usd, US Dollar → USD). Ensure consistent date formatting.

## Step 2: Data Analysis
After cleaning, analyze the dataset to extract meaningful insights.

- Calculate total sales:
  Determine total revenue from all products.

- Calculate profit margin:
  Profit margin is calculated as profit divided by sales amount multiplied by 100.

- Currency conversion:
  Research exchange rates and convert all currencies to a single base currency such as USD.

- Handle missing or incorrect values:
  Decide whether to exclude or adjust records with missing or extreme values such as negative profit.

## Step 3: Data Modeling
Structure the data for efficient analysis.

- Create dimension tables:
  Include tables for products, customers, locations, and time.

- Create fact table:
  Store transactional data such as OrderID, SalesAmount, Profit, Quantity, and Discount.

- Create relationships:
  Link the fact table to dimension tables using appropriate keys.

- Create time dimension:
  Include Year, Quarter, Month, Week, Day, and Date for time-based analysis.

## Step 4: Building the Dashboard
Create an interactive dashboard to present insights.

- Key visualizations:
  KPI cards for total sales, total profit, and profit margin.
  Bar or column charts for sales by product or region.
  Line charts for sales trends over time.
  Pie charts for sales distribution.
  Map visuals for geographical insights.

- Use slicers:
  Add filters for year, region, product category, and customer.

## Step 5: Creating the Report
Develop a detailed report with insights.

- Executive summary:
  Provide an overview of sales performance, top products, and profitability.

- Detailed analysis:
  Analyze sales by region, product performance, and trends over time.

- Visual insights:
  Answer key questions such as top-performing products, highest profit regions, and sales trends.

- Recommendations:
  Suggest actions such as promoting high-performing products and improving low-profit regions.

## Report Structure in Power BI

- Reports contain multiple pages.
- Each page focuses on a specific analysis area.
- The first page acts as the main dashboard.
- Additional pages provide detailed insights.

### Example Pages
- Sales overview
- Product performance
- Geographical analysis
- Customer insights

## Navigation
Users can move between pages using tabs or buttons. Navigation buttons like "Next Page" or "Back to Dashboard" can improve usability.

## Steps to Organize Pages

- Create new pages using the "+" button.
- Rename pages appropriately.
- Design the first page with KPIs and visuals.
- Create additional pages for deeper analysis.
- Add navigation buttons for interactivity.

## Key Analytical Questions
- How do exchange rates affect sales?
- Should missing values be excluded or filled?
- Do higher discounts increase engagement?
- How should repeat customers be analyzed?

## Conclusion
This project demonstrates the full Power BI workflow including data cleaning, analysis, modeling, and visualization. The final output is a comprehensive dashboard and report that provides meaningful insights into the electronics sales business.


## PROJECT SOLUTIONs
**Data Cleaning**
* **OrderDate is in Date data type**
<img width="950" height="482" alt="image" src="https://github.com/user-attachments/assets/a85b63c0-7567-4d4f-bfba-901ff12a5e9a" />

* **No missing Data**
* **No Pseudonyms and Invalid Entries**
* **Data is in correct Formats**
* **No spelling Errors**

  ### Data Analysis
  
  Use **DAX (Data Analysis Expressions)** to derive key insights.
  
  * **Calculate Total Sales**
    
    ```Total Sales = SUM(Electronics_Sales[SalesAmount])```
    
    <img width="953" height="475" alt="image" src="https://github.com/user-attachments/assets/6fb2d234-d1c4-4c5c-9b4d-fe5a388c89f9" />

    * **Profit Margin Calculation**

      ```Profit Margin = DIVIDE(SUM(Electronics_Sales[Profit]), SUM(Electronics_Sales[SalesAmount])) * 100```
      
      <img width="954" height="363" alt="image" src="https://github.com/user-attachments/assets/3a3e3f97-3315-4a6a-acc0-ade683a4f44d" />

      **Currency Conversion**
      
      <img width="959" height="380" alt="image" src="https://github.com/user-attachments/assets/78d96653-dfd5-42b8-ab36-3c567005ef1f" />

    ### Data Modeling
      * **Create Dimension Tables**
   
        <img width="911" height="469" alt="image" src="https://github.com/user-attachments/assets/5b62755d-6d4c-4d4b-be80-4221a865a598" />

### Building the Dashboard

**The following Dashboard Represents**
* Total Sales
* Total Profit
* Profit Margin
* Bar and Column chart representing Sales by product, Region and Category

  <img width="959" height="479" alt="image" src="https://github.com/user-attachments/assets/cfbd971a-b3ef-4d3e-93e4-cfce558a7516" />

  **The following Dashboard Represents**
  * Sales Trends By Month
  * Sales Distribution By Currency
  * Sales Distribution By City(Visual Map)
  * Slicers By Customer, Product Category, and Time Period
 
    <img width="959" height="470" alt="image" src="https://github.com/user-attachments/assets/f523ac0d-f157-4abf-a3a2-a481fe0b7bd1" />


    

        
      
      


    




