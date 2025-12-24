# Anand Ecommerce Sales Dashboard
## Interactive Power BI Analytics Solution    
Comprehensive sales performance analysis across regions, customers, categories, and profitability trends

## Project Overview

Professional Power BI dashboard analyzing ecommerce sales performance across 882 orders worth ₹87K with 1,181 units sold. Enables business stakeholders to track regional performance, customer contributions, payment trends, and profit drivers through interactive visualizations and DAX-powered KPIs.

### Business Objectives
**Core Challenges Addressed:**

1. Identify top-performing regions and customer segments

2. Analyze product profitability by category/sub-category

3. Track payment method preferences and adoption trends

4. Monitor monthly profit fluctuations for operational optimization

### Key Deliverables:
1. **Total Sales:** ₹87,000                         
2. **Total Orders:** 882                                     
3. **Total Quantity:** 1,181 units                                         
4. **Primary Metrics:** Sales Amount | Profit | Order Volume | Customer Contribution                       

## Technical Stack
1. **Visualization:** Power BI Desktop - Interactive dashboard creation
2. **Data Prep:** Power Query - ETL, cleaning, transformation
3. **Calculations:** DAX - KPIs, dynamic measures, slicers
4. **Data Model:** Star Schema - Multi-table relationships
5. **Output:** .pbix - Deployable dashboard file
   
### Dataset Structure
**Source:** Simulated Ecommerce Sales Dataset

**Key Dimensions:**
1. **Orders:** Sales, Profit, Quantity, Date (₹87K total sales)
2. **Geography:** State (Maharashtra, Madhya Pradesh)
3. **Customers:** Customer Name (Vrinda, Priyanka, Bhawna)
4. **Products:** Category, Sub-Category (Clothing/Trousers, Furniture/Tables)
5. **Payments:** Payment Mode (COD, UPI, Cards, EMI

## Dashboard Features
**1. Executive KPI Cards (Top Row)**                                           
Total Sales Amount: ₹87,000           
Total Orders: 882                            
Total Quantity Sold: 1,181 units                              
Profit Summary: Mixed (April peak, May dip)                            

**2. Regional Performance**                                      
Sales by State (Bar Chart)                                                    
Maharashtra: Highest revenue contributor                                                              
Madhya Pradesh: Strong secondary market                                                             
Others: Growth opportunities                                                      

**3. Product Analytics**                                         
Quantity by Category (Donut Chart)                                                          
Clothing: 61% dominance                                                 
Electronics: 23%                                                                  
Furniture: 16%
                                          
Profit by Sub-Category (Bar Chart)                             
Top Performers: Tables, Printers                                    
Low Margin: Trousers, Shirts                                                               
                                              
**4. Customer & Payment Insights**                                               
Top Customers (Bar Chart)                                                             
Vrinda: #1 revenue driver                                                             
Priyanka & Bhawna: Key accounts                                                                             

Payment Mode (Donut Chart)                                     
COD: 44% preference                                
UPI: 21% (digital growth)                                  
Cards/EMI: 25% combined                                   

**5. Time Series Analysis**                                                  
Profit by Month (Bar Chart)                                             
April: Profit peak                                            
May: Concerning dip (investigate)                                           
June: Recovery trend                                      

## Key DAX Measures
```sql, python, dax
Total Sales = SUM(Orders[Sales Amount])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
YoY Growth = 
    VAR CurrentYear = SUM(Orders[Sales Amount])
    VAR PrevYear = CALCULATE(SUM(Orders[Sales Amount]), SAMEPERIODLASTYEAR(Orders[Order Date]))
    RETURN DIVIDE(CurrentYear - PrevYear, PrevYear, 0)
```
 ## Business Impact
1. **Revenue Optimization:** Target high-profit sub-categories (Tables/Printers)
2. **Regional Strategy:** Double down on Maharashtra/MP expansion
3. **Customer Focus:** Loyalty programs for top 3 customers
4.**Payment Shift:** UPI promotion to reduce COD dependency
5. **Profit Recovery:** May loss investigation & corrective action

### Interactive Capabilities
1. **Slicers:** State | Category | Month | Payment Mode
2. **Cross-Filtering:** Click any visual to drill down
3. **Drill-Through:** Customer/Product deep dives
4. **Tooltips:** Detailed metrics on hover
5. **Mobile Optimized:** Responsive design

### Deployment Guide
Download Anand-Ecommerce-Sales-Dashboard.pbix                      

Open in Power BI Desktop                     

Refresh data connections              

Publish to Power BI Service (optional)                           

Share via app/workspace                          








