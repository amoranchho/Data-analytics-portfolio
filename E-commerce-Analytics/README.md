E-Commerce Data Cleaning Project
📌 Project Overview

This project focused on cleaning and preparing an E-Commerce dataset for analysis and dashboard development. The goal was to improve data quality, ensure consistency, handle missing values, and create a reliable dataset for business intelligence reporting in Power BI.

🎯 Objectives
Remove duplicate records
Standardize text and date formats
Handle missing values
Improve data consistency
Prepare data for analysis and visualization
📊 Dataset Summary
Metric	Value
Original Records	5,000
Duplicate Records Removed	30
Records Dropped (Critical Missing Values)	40
Final Dataset Size	4,930
🔧 Data Cleaning Steps
1. Duplicate Records
Identified duplicate Order IDs.
Removed duplicate entries while retaining the first occurrence.

Records Removed: 30

2. Date Standardization

Multiple date formats were found, including:

DD/MM/YYYY
YYYY-MM-DD
Other inconsistent formats

Action Taken:

Standardized all dates to DD/MM/YYYY format.
3. Text Standardization

Several categorical fields contained inconsistent capitalization and naming conventions.

Customer Segment

Examples:

vip
VIP
New customer

Standardized to:

VIP
New Customer
Returning Customer
Shipping Method

Standardized to:

Free Shipping
Standard
Express
Next Day
Payment Method

Standardized to:

PayPal
Credit Card
Debit Card
Bank Transfer
Order Status

Standardized to:

Completed
Pending
Shipped
Returned
Cancelled
Return Requested

Standardized to:

Yes
No
Stock Status

Standardized to:

In Stock
Low Stock
Out Of Stock
Unknown
4. Missing Value Treatment
Column	Missing Values	Action Taken
Return Requested	256	Filled with "No"
Stock Status	253	Filled with "Unknown"
Discount	25	Filled with 0
Revenue	65	Recalculated using Price × Quantity × (1 - Discount)
Customer ID	35	Filled with "UNKNOWN"
Delivery Days	13	Filled with Median Value
Product Rating	14	Filled with Median Value
5. Removing Invalid Records

Rows with missing critical business fields were removed:

Revenue
Quantity
Price

Rows Removed: 40

✅ Final Outcome

The dataset is now:

✔ Free from duplicates

✔ Consistent in formatting

✔ Standardized across categories

✔ Missing values appropriately handled

✔ Ready for exploratory analysis and dashboard creation

🛠️ Tools Used
Microsoft Excel
Data Cleaning Techniques
Data Validation
Business Rules & Standardization
📈 Next Phase

The cleaned dataset will be used to develop an interactive Power BI dashboard covering:

Sales Performance
Customer Insights
Product Analysis
Shipping & Return Trends
Revenue and Profit KPIs
